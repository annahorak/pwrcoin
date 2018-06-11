# Constants

Changes in NXT source code will mainly depend on modifying constants defining behavior of cryptocurrency. Below you can find all important constants which are modified in PWrCoin.

### All of these constants can be find in Constants.java file

```java
 // Maximum amount of transactions per block
 public static final int MAX_NUMBER_OF_TRANSACTIONS = 255;
```

```java
// Maximum amount of coins
public static final long MAX_BALANCE_NXT = 1000000000;
```

```java
// Precision of one coin
public static final long ONE_NXT = 100000000;
```

```java
 // Minimum and maximum time of block creation
 public static final int MIN_BLOCKTIME_LIMIT = 53;
 public static final int MAX_BLOCKTIME_LIMIT = 67;
```

```java
// Minimum and maximum weights of vote
public static final byte MIN_VOTE_VALUE = -92;
public static final byte MAX_VOTE_VALUE = 92;
public static final byte NO_VOTE_VALUE = Byte.MIN_VALUE;
```

```java
 // Initiation date of cryptocurrency life (ability of manipulation during creation new crypto each year)
 public static final long EPOCH_BEGINNING;
 static {
  Calendar calendar = Calendar.getInstance(TimeZone.getTimeZone("UTC"));
  calendar.set(Calendar.YEAR, 2013);
  calendar.set(Calendar.MONTH, Calendar.NOVEMBER);
  calendar.set(Calendar.DAY_OF_MONTH, 24);
  calendar.set(Calendar.HOUR_OF_DAY, 12);
  calendar.set(Calendar.MINUTE, 0);
  calendar.set(Calendar.SECOND, 0);
  calendar.set(Calendar.MILLISECOND, 0);
  EPOCH_BEGINNING = calendar.getTimeInMillis();
  }
```



