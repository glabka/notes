* probably not important but might be handy to learn gradle

# HackerRank
* (java) Please do not use any package names in your code.

## what I have learned
* printf
### regex
* Pattern p = Patter.compile("regex") -> p.matcher(string) -> p.find() -> p.group(index / name)
### concurrency
* https://docs.oracle.com/javase/tutorial/essential/concurrency/collections.html - BlockingQueue, ConcurrentHashMap, ConcurrentSkipListMap
* Collections.synchronizedCollection(Collection<T> c) -> returns Collection<T>
### other
* how to do Integer[] from int[]: int[] arr ... -> Integer[] boxedArr = Arrays.stream(arr).boxed().toArray( Integer[]::new)
* how to do List<Integer> from int[]: int[] arr ... -> Integer[] boxedArr = Arrays.stream(arr).boxed().collect(Collectors.toList());
* Binary numeric promotion is performed on the operands (§5.6.2). -> adding short and short -> result is int so has to be explicitly cast back to short
* System.arraycopy
* Arrays.sort - HackerRank občas nenašeptává metody, co existují
* new String(bytes)
* BigIngeger.valueOf((long) 8); sum methods returns new BigInteger
* value of letter without "offset": 'B' - 'A'
* Arrays.fill(array, value)
* List l = ...; -> l.subList(0, 3);
#### byte array to Byte List
* there is not a boxed method for stream of bytes
```
        byte[] someBytes = {(byte) 1,(byte) 2,(byte) 3,(byte) 4,(byte) 5,(byte) 6,(byte) 7,(byte) 8,(byte) 9,(byte) 10};
        Byte[] bytesBoxed = new Byte[10];
        Arrays.setAll(bytesBoxed, n -> someBytes[n]);
        System.out.println(Arrays.stream(bytesBoxed).collect(Collectors.toList()));
```  
