public interface ITriggerHandler {
    
    void onBeforeInsert(List<SObject> newItems);
    void onBeforeUpdate(Map<Id, SObject> newItems, Map<Id, SObject> oldItems);
    void onBeforeDelete(Map<Id, SObject> deletedSObjects);
    void onAfterInsert(Map<Id, SObject> newItems);
    void onAfterUpdate(Map<Id, SObject> newItems, Map<Id, SObject> oldItems);
    void onAfterDelete(Map<Id, SObject> newItems);
    void onAfterUnDelete(Map<Id, SObject> newItems);
    
}