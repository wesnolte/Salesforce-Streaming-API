# Push Notifications Demo for Salesforce

You will also need a Push Topic some like this:

    PushTopic pushTopic = new PushTopic();
    pushTopic.Name = 'AllAccounts';
    pushTopic.Query = 'SELECT id, name FROM Account';
    pushTopic.ApiVersion = 26.0;
    pushTopic.NotifyForOperations = 'All';
    pushTopic.NotifyForFields = 'Referenced';
    insert pushTopic;