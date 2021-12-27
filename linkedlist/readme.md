1.Cycle detection in linkedlist 
## Using Two pointer
def has_cycle(head):

    slow = fast = head
    while fast!=None and fast.next!=None:
    #increase the slow and fast value
          slow = slow.next
          fast = fast.next.next
    #Check the condition
          if slow == fast:
            return True
    return False
## Using HashSet
   visited = set()
    f = head
    while f:
        i = id(f)
        if i in visited:
            return 1
        visited.add(i)
        f = f.next
    return 0
##Using Dictionary 
pos = {head: 0};
    
    while head.next:
        if head.next in pos:
            return 1
        pos[head.next] = 0
        head = head.next
    
    return 0
2.Delete duplicate from linkedlist

def removeDuplicates(llist):
    # Write your code here
    temp = llist
    while temp.next!=None:
        if temp.data == temp.next.data:
            temp.next = temp.next.next
        else:
            temp = temp.next
    return llist

    #  Find Merge Point of Two Lists | Linked List |
    def findMergeNode(head1, head2):
    def get_count(head):
        n = 0
        while head.next!=None:
            head = head.next
            n += 1
        return n
    def get_Node(d,head1,head2):
        for i in range(d):
            head1 = head1.next
        while head1 and head2:
            if head1 == head2:
                return head1.data
            else:
                head1 = head1.next
                head2 = head2.next
        
    c1 = get_count(head1)
    c2 = get_count(head2)
    if c1 > c2 :
        return get_Node(c1 - c2,head1,head2)
    else: 
        return get_Node(c2-c1, head2,head1)