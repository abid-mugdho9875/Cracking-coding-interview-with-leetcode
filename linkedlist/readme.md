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