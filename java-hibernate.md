# Hibernate


#### Annotations

* **@Temporal** - In plain Java APIs, the temporal precision of time is not defined. When dealing with temporal data, you might want to describe the expected precision in database. Temporal data can have DATE, TIME, or TIMESTAMP precision (i.e., the actual date, only the time, or both). Use the _@Temporal_ annotation to fine tune that.
* **@OneToMany** - указывающей на наличие отношения “один ко многим”
  * **mappedBy** - которое предоставляет ассоциацию (т.е. связано с определением внешнего ключа в таблице)
  * **cascade** - означает, что операция обновления должна распространяться на дочерние записи.
  * **orphanRemoval** - что после обновления chiulde записи, которые больше не существуют в наборе, должны быть удалены из базы данных.
  * **fetch** - 
      * LAZY - fetch when needed
      * EAGER - fetch immediately
* **@LazyCollection**
  * **LazyCollectionOption.FALSE** - Eager-Loading
  * **LazyCollectionOption.TRUE** - initialize the whole collection on first access
  * **LazyCollectionOption.EXTRA** - .size() and .contains() won't initialize the whole collection
