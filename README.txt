TestPerformance Results

SIZE 10

ArrayList AddRemove: 223 ms
LinkedList AddRemove: 14 ms
ArrayList Access: 7 ms
LinkedList Access: 6 ms

SIZE 100

ArrayList AddRemove: 254 ms
LinkedList AddRemove: 14 ms
ArrayList Access: 8 ms
LinkedList Access: 12 ms

SIZE 1000

ArrayList AddRemove: 67 ms
LinkedList AddRemove: 8 ms
ArrayList Access: 7 ms
LinkedList Access: 45 ms

SIZE 10000

ArrayList AddRemove: 21 ms
LinkedList AddRemove: 5 ms
ArrayList Access: 4 ms
LinkedList Access: 54 ms

Conclusion:
1. For Access (get):
    ArrayList is much faster than LinkedList
    Difference becomes larger as the size increases.

2. For Add/Remove at index 0:
   LinkedList performs better than ArrayList.
   This is because ArrayList must shift elements when inserting or removing at the beginning.

3. As the list size increases:
     ArrayList becomes significantly better for access operations.
     LinkedList remains better for add/remove at the front.

Behavioral Comparison (ArrayList vs LinkedList):

I replaced ArrayList with LinkedList in TestList and TestIterator and ran all tests again.
  All tests still passed successfully.

There is no behavioral difference between ArrayList and LinkedList for the List operations tested.
The difference between them is in performance, not behavior.