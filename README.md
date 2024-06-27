public class BalanceTransferWrapper {
    public class BalanceTransfer {
        public Integer balanceTransferId;
        public Integer accountId;
        public Integer customerId;
        public Decimal amount;
        public String channelType;
        public Integer externalAccountId;
        public String insertUser;
        public Datetime insertTimestamp;
        public Datetime balanceTransferDate;
        public String balanceTransferType;
        public String securityCode;
        public String statusForCustomer;
        public String status;
        public String statusReason;
        public String statusReasonForCustomer;
        public String applicationSeqId;
        public Integer eomOfferTrackId;
        public Integer referenceNbr;
        public Integer transNbr;
        public String modUser;
        public Datetime modTimestamp;
        public Datetime reqTimestamp;
        public String accountNumber;
        public String externalAccountNumber;
        public String bankName;
        public Integer routingNumber;
    }
    
    public List<BalanceTransfer> balanceTransfer;
}


<template>
    <lightning-card>
        <div class="slds-grid slds-wrap">
            <!-- First Column -->
            <div class="slds-col slds-size_1-of-2 slds-p-around_medium">
                <div class="slds-grid slds-wrap slds-grid_align-spread">
                    <div class="slds-col slds-size_1-of-2 slds-text-align_right">
                        Key 1:
                    </div>
                    <div class="slds-col slds-size_1-of-2 slds-text-align_left">
                        Value 1
                    </div>
                </div>
                <div class="slds-grid slds-wrap slds-grid_align-spread">
                    <div class="slds-col slds-size_1-of-2 slds-text-align_right">
                        Key 2:
                    </div>
                    <div class="slds-col slds-size_1-of-2 slds-text-align_left">
                        Value 2
                    </div>
                </div>
                <!-- Add more key-value pairs as needed -->
            </div>
            <!-- Second Column -->
            <div class="slds-col slds-size_1-of-2 slds-p-around_medium">
                <div class="slds-grid slds-wrap slds-grid_align-spread">
                    <div class="slds-col slds-size_1-of-2 slds-text-align_right">
                        Key A:
                    </div>
                    <div class="slds-col slds-size_1-of-2 slds-text-align_left">
                        Value A
                    </div>
                </div>
                <div class="slds-grid slds-wrap slds-grid_align-spread">
                    <div class="slds-col slds-size_1-of-2 slds-text-align_right">
                        Key B:
                    </div>
                    <div class="slds-col slds-size_1-of-2 slds-text-align_left">
                        Value B
                    </div>
                </div>
                <!-- Add more key-value pairs as needed -->
            </div>
        </div>
    </lightning-card>
</template>






