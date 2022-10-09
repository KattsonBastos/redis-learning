# Redis Basic Data Types

<a href="https://github.com/KattsonBastos/redis-learning/#contents">Back to Contents</a>

<p align="justify">
&ensp;&ensp;&ensp;&ensp;Redis supports not only string-string pairs, but many other data structures. This note covers the 5 basic data structures it supports: <strong>Strings, Lists, Sets, Sorted Sets, and Hashes</strong>.
</p>



---
# Strings
It's just a sequence of bytes. Since it is the only Redis data type that is `Memcached`, it's the only one we can use for web pages.

Since it stores a sequence of bytes, a String could be text, binary arrays, and any other serialzied objects.

---
# Lists
This is another simple data structure. A list in Redis is just a collection or strings sorted by the insertion order of the items. They are mainly used for stacking and queuing.

---
# Sets
Sets are very similar to List, but they are an unordered collection of strings. According to the [Redis Documentation](https://redis.io/docs/data-types/sets/), we can add, remove, and test for members existence in O(1) time complexity. that means it does not matter the number of items in the set.

---
# Sorted Sets
They are similar to sets, but each element is associated with a score. So, we can use it, for example, in Leaderboards, where we can easily sort and get the top/bottom elements.

---
# Hashes
Redis Hashes are a collection of field-value pairs. So, we could use it to store a lot of information from a user, such as the login, address, personal info, and so on.