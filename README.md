# Middle-of-the-Linked-List-leetcode

class Solution {

    public ListNode middleNode(ListNode head) {

      ListNode hare = head;
     ListNode tail = head;
     while(hare != null && hare.next !=null){
         hare = hare.next.next;
         tail = tail.next;
         if(hare == tail ){
             return tail.next;
         }
     }
     return tail;
}
}
