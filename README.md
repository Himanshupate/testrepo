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
