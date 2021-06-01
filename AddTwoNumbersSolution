/**
 * Definition for singly-linked list.
 * public class ListNode {
 *     int val;
 *     ListNode next;
 *     ListNode() {}
 *     ListNode(int val) { this.val = val; }
 *     ListNode(int val, ListNode next) { this.val = val; this.next = next; }
 * }
 */
class AddTwoNumbersSolution {
    int carry = 0;
    
    public ListNode addTwoNumbers(ListNode l1, ListNode l2) {
        ListNode result = null;
        ListNode temp = null;
            
        while(true){
            int sum = carry;
            carry = 0;

            if (l1 != null){
                sum = sum + l1.val;
                l1 = l1.next;

            }

            if (l2 != null){
                sum = sum + l2.val;
                l2 = l2.next;
            }

            if (sum > 9){
                carry = 1;
                sum = sum - 10;
            }
            
            if (temp != null){
                temp.next = new ListNode(sum);
                temp = temp.next;
            }
            else {
                temp = new ListNode(sum);
            }
            
            if (l1 == null && l2 == null){
                if (carry !=0){
                    temp.next = new ListNode(1);
                }
                if (result == null){
                    result = temp;
                }
                break;
                
            }
            if (result == null){
                    result = temp;
                }
            
        }
        
        return result;
    }
}
