# testrepo
This is the test repository for devops.
public class SoapWebServiceCallout {

    // Define the endpoint URL of the SOAP web service
    private static final String ENDPOINT_URL = 'https://example.com/soap/service';

    // Define the SOAP action
    private static final String SOAP_ACTION = 'http://example.com/soap/action';

    // Define the request XML
    private static final String REQUEST_XML = '<soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:web="http://example.com/namespace">'
                                                + '<soapenv:Header/>'
                                                + '<soapenv:Body>'
                                                + '<web:MethodName>'
                                                + '<web:Parameter1>Value1</web:Parameter1>'
                                                + '<web:Parameter2>Value2</web:Parameter2>'
                                                + '</web:MethodName>'
                                                + '</soapenv:Body>'
                                                + '</soapenv:Envelope>';

    // Method to make the SOAP callout
    public static void makeCallout() {
        HttpRequest httpRequest = new HttpRequest();
        httpRequest.setEndpoint(ENDPOINT_URL);
        httpRequest.setMethod('POST');
        httpRequest.setHeader('Content-Type', 'text/xml');
        httpRequest.setHeader('SOAPAction', SOAP_ACTION);
        httpRequest.setBody(REQUEST_XML);
        
        // Create a new HTTP object to send the request
        Http http = new Http();
        HttpResponse httpResponse = http.send(httpRequest);
        
        // Process the response
        if (httpResponse.getStatusCode() == 200) {
            // Success - handle the response here
            String responseBody = httpResponse.getBody();
            System.debug('Response: ' + responseBody);
        } else {
            // Error handling
            System.debug('Error: HTTP request failed with status code ' + httpResponse.getStatusCode());
        }
    }
}
