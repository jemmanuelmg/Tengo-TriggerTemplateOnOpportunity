public class TriggerDispatcher {
    
    public static void run(ITriggerHandler handler) {
        
        if (Trigger.IsBefore) {
            
            if (Trigger.IsInsert) {
                handler.onBeforeInsert(trigger.new);
                
            } else if (Trigger.IsUpdate) {
                handler.onBeforeUpdate(trigger.newMap, trigger.oldMap);
                
            } else if (Trigger.IsDelete) {
                handler.onBeforeDelete(trigger.oldMap);
                
            }
        }
        
        if (Trigger.IsAfter) {
            
            if (Trigger.IsInsert) {
                handler.onAfterInsert(Trigger.newMap);
                
            } else if (Trigger.IsUpdate) {
            	handler.onAfterUpdate(trigger.newMap, trigger.oldMap);
                
            } else if (trigger.IsDelete) {
                handler.onAfterDelete(trigger.oldMap);
                
            } else if (trigger.isUndelete) {
                handler.onAfterUndelete(trigger.oldMap);
                
            }
        }
    }
}