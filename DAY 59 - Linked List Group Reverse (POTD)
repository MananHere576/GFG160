class Solution {
    public static Node reverseKGroup(Node head, int k) {
        // code here
        if(head==null) return head;
        if(len(head)<k) return rev(head);
        Node curr=head,next=null,prev=null;
        for(int i=0;i<k;i++){
           next=curr.next;
           curr.next=prev;
           prev=curr;
           curr=next;
        }
        head.next=reverseKGroup(curr,k);
        return prev;
    }
    private static int len(Node head){
        int n=0;
        while(head!=null){
            n++;
            head=head.next;
        }
        return n;
    }
    private static Node rev(Node head){
        Node curr=head,next=null,prev=null;
        while(curr!=null){
           next=curr.next;
           curr.next=prev;
           prev=curr;
           curr=next;
        }
        return prev;
    }
}
