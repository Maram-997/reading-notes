# Read - 10 : Queues And Stacks

## Stack : 
A stack is a data structure that consists of Nodes. Each Node references the next Node in the stack, but does not reference its previous.

#### Stacks follow these concepts :
**FILO** First In Last Out
>This means that the first item added in the stack will be the last item popped out of the stack.

**LIFO** Last In First Out
>This means that the last item added to the stack will be the first item popped out of the stack.

#### Stack Methods :
* push : to add new element to the stack (it will be added as first element)
* pop : to remove an element from the stack (the last one wes added will be removed)

>Head : This is the front/first Node of the queue.
>Tail : This is the rear/last Node of the queue.
 

## Queue :
is a linear structure which follows a particular order in which the operations are performed. 

#### Queues follow these concepts : 
**FIFO** First In First Out
>This means that the first item in the queue will be the first item out of the queue.

**LILO** Last In Last Out
>This means that the last item in the queue will be the last item out of the queue.

#### Queue Methods : 
* enqueue : to add new element to the queue (it will be added as the last element in the queue)
* dequeue : to remove an element from the queue (the first one in the queue will be removed)

>Front : This is the front/first Node of the queue.
>Rear : This is the rear/last Node of the queue.

## **Common Methods between queues and stacks**
Peek : When you peek you will view the `value` of the top Node in the stack. When you attempt to peek an empty stack an exception will be raised.