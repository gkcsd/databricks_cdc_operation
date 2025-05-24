# databricks_cdc_operation


-------------------------------------------
Batch: 0
-------------------------------------------
+--------------+------+-----------+------------------+---------------------+------------------+------------+---------------+-----------------+
|transaction_id|upi_id|merchant_id|transaction_amount|transaction_timestamp|transaction_status|_change_type|_commit_version|_commit_timestamp|
+--------------+------+-----------+------------------+---------------------+------------------+------------+---------------+-----------------+
+--------------+------+-----------+------------------+---------------------+------------------+------------+---------------+-----------------+

2025-05-24T13:11:34.989+0000: [GC (Allocation Failure) [PSYoungGen: 1446275K->33968K(1523200K)] 1620739K->208440K(4785152K), 0.0383272 secs] [Times: user=0.06 sys=0.00, real=0.03 secs] 
2025-05-24T13:11:42.987+0000: [GC (Allocation Failure) [PSYoungGen: 1452720K->45473K(1535488K)] 1627192K->219952K(4797440K), 0.0919832 secs] [Times: user=0.12 sys=0.00, real=0.10 secs] 
2025-05-24T13:11:45.870+0000: [GC (Allocation Failure) [PSYoungGen: 1481121K->95216K(1530880K)] 1655600K->272837K(4792832K), 0.0474668 secs] [Times: user=0.08 sys=0.00, real=0.04 secs] 
2025-05-24T13:11:51.832+0000: [GC (Allocation Failure) [PSYoungGen: 1530864K->49302K(1520640K)] 1708485K->226931K(4782592K), 0.0711321 secs] [Times: user=0.13 sys=0.00, real=0.07 secs] 
Batch processed successfully.
-------------------------------------------
Batch: 1
-------------------------------------------
+--------------+---------+-----------+------------------+---------------------+------------------+------------+---------------+--------------------+
|transaction_id|   upi_id|merchant_id|transaction_amount|transaction_timestamp|transaction_status|_change_type|_commit_version|   _commit_timestamp|
+--------------+---------+-----------+------------------+---------------------+------------------+------------+---------------+--------------------+
|          T001|upi1@bank|       M001|             500.0|  2024-12-21 10:00:00|         initiated|      insert|              1|2025-05-24 13:11:...|
|          T002|upi2@bank|       M002|            1000.0|  2024-12-21 10:05:00|         initiated|      insert|              1|2025-05-24 13:11:...|
|          T003|upi3@bank|       M003|            1500.0|  2024-12-21 10:10:00|         initiated|      insert|              1|2025-05-24 13:11:...|
+--------------+---------+-----------+------------------+---------------------+------------------+------------+---------------+--------------------+

2025-05-24T13:14:16.088+0000: [GC (Allocation Failure) [PSYoungGen: 1470102K->53654K(1525760K)] 1647731K->231291K(4787712K), 0.1245631 secs] [Times: user=0.09 sys=0.00, real=0.13 secs] 
2025-05-24T13:14:24.484+0000: [GC (Allocation Failure) [PSYoungGen: 1474454K->61977K(1529856K)] 1652091K->239622K(4791808K), 0.0604891 secs] [Times: user=0.11 sys=0.00, real=0.06 secs] 
Batch processed successfully.
2025-05-24T13:14:30.757+0000: [GC (Allocation Failure) [PSYoungGen: 1490457K->66753K(1495552K)] 1668102K->244406K(4757504K), 0.0613993 secs] [Times: user=0.11 sys=0.00, real=0.06 secs] 
-------------------------------------------
Batch: 2
-------------------------------------------
+--------------+---------+-----------+------------------+---------------------+------------------+----------------+---------------+--------------------+
|transaction_id|   upi_id|merchant_id|transaction_amount|transaction_timestamp|transaction_status|    _change_type|_commit_version|   _commit_timestamp|
+--------------+---------+-----------+------------------+---------------------+------------------+----------------+---------------+--------------------+
|          T001|upi1@bank|       M001|             500.0|  2024-12-21 10:00:00|         initiated| update_preimage|              2|2025-05-24 13:14:...|
|          T001|upi1@bank|       M001|             500.0|  2024-12-21 10:15:00|         completed|update_postimage|              2|2025-05-24 13:14:...|
|          T002|upi2@bank|       M002|            1000.0|  2024-12-21 10:05:00|         initiated| update_preimage|              2|2025-05-24 13:14:...|
|          T002|upi2@bank|       M002|            1000.0|  2024-12-21 10:20:00|            failed|update_postimage|              2|2025-05-24 13:14:...|
|          T004|upi4@bank|       M004|            2000.0|  2024-12-21 10:25:00|         initiated|          insert|              2|2025-05-24 13:14:...|
+--------------+---------+-----------+------------------+---------------------+------------------+----------------+---------------+--------------------+

2025-05-24T13:14:37.265+0000: [GC (Allocation Failure) [PSYoungGen: 1495233K->72709K(1522688K)] 1672886K->250370K(4784640K), 0.0999488 secs] [Times: user=0.12 sys=0.01, real=0.10 secs] 
-------------------------------------------
Batch: 3
-------------------------------------------
+--------------+------+-----------+------------------+---------------------+------------------+------------+---------------+-----------------+
|transaction_id|upi_id|merchant_id|transaction_amount|transaction_timestamp|transaction_status|_change_type|_commit_version|_commit_timestamp|
+--------------+------+-----------+------------------+---------------------+------------------+------------+---------------+-----------------+
+--------------+------+-----------+------------------+---------------------+------------------+------------+---------------+-----------------+

2025-05-24T13:15:59.075+0000: [GC (Allocation Failure) [PSYoungGen: 1493509K->66875K(1525760K)] 1671170K->244544K(4787712K), 0.0635983 secs] [Times: user=0.11 sys=0.00, real=0.06 secs] 
2025-05-24T13:18:28.519+0000: [GC (Allocation Failure) [PSYoungGen: 1481064K->72555K(1523200K)] 1658733K->250232K(4785152K), 0.0779604 secs] [Times: user=0.13 sys=0.00, real=0.07 secs] 
2025-05-24T13:18:34.155+0000: [GC (Allocation Failure) [PSYoungGen: 1491307K->77790K(1496576K)] 1668984K->255475K(4758528K), 0.0734846 secs] [Times: user=0.13 sys=0.00, real=0.07 secs] 
Batch processed successfully.
-------------------------------------------
Batch: 4
-------------------------------------------
+--------------+---------+-----------+------------------+---------------------+------------------+----------------+---------------+--------------------+
|transaction_id|   upi_id|merchant_id|transaction_amount|transaction_timestamp|transaction_status|    _change_type|_commit_version|   _commit_timestamp|
+--------------+---------+-----------+------------------+---------------------+------------------+----------------+---------------+--------------------+
|          T001|upi1@bank|       M001|             500.0|  2024-12-21 10:15:00|         completed| update_preimage|              4|2025-05-24 13:18:...|
|          T001|upi1@bank|       M001|             500.0|  2024-12-21 10:30:00|          refunded|update_postimage|              4|2025-05-24 13:18:...|
|          T003|upi3@bank|       M003|            1500.0|  2024-12-21 10:10:00|         initiated| update_preimage|              4|2025-05-24 13:18:...|
|          T003|upi3@bank|       M003|            1500.0|  2024-12-21 10:35:00|         completed|update_postimage|              4|2025-05-24 13:18:...|
+--------------+---------+-----------+------------------+---------------------+------------------+----------------+---------------+--------------------+

2025-05-24T13:18:39.682+0000: [GC (Allocation Failure) [PSYoungGen: 1496542K->83592K(1513472K)] 1674227K->261285K(4775424K), 0.0930386 secs] [Times: user=0.14 sys=0.00, real=0.09 secs] 
-------------------------------------------
Batch: 5
-------------------------------------------
+--------------+------+-----------+------------------+---------------------+------------------+------------+---------------+-----------------+
|transaction_id|upi_id|merchant_id|transaction_amount|transaction_timestamp|transaction_status|_change_type|_commit_version|_commit_timestamp|
+--------------+------+-----------+------------------+---------------------+------------------+------------+---------------+-----------------+
+--------------+------+-----------+------------------+---------------------+------------------+------------+---------------+-----------------+

2025-05-24T13:19:36.970+0000: [GC (Allocation Failure) [PSYoungGen: 1488008K->76306K(1481216K)] 1665701K->254007K(4743168K), 0.0712469 secs] [Times: user=0.12 sys=0.01, real=0.07 secs] 
2025-05-24T13:21:01.025+0000: [GC (System.gc()) [PSYoungGen: 580754K->66367K(1521152K)] 758455K->247262K(4783104K), 0.0649863 secs] [Times: user=0.12 sys=0.00, real=0.07 secs] 
2025-05-24T13:21:01.090+0000: [Full GC (System.gc()) [PSYoungGen: 66367K->0K(1521152K)] [ParOldGen: 180894K->206139K(3261952K)] 247262K->206139K(4783104K), [Metaspace: 482826K->478741K(1538048K)], 1.1382781 secs] [Times: user=1.87 sys=0.02, real=1.13 secs] 
2025-05-24T13:23:50.473+0000: [GC (Allocation Failure) [PSYoungGen: 1407488K->18821K(1517056K)] 1613627K->224969K(4779008K), 0.0266680 secs] [Times: user=0.04 sys=0.01, real=0.03 secs] 
DELTA TABLE 'INCREMENTAL_LOAD.DEFAULT.RAW_UPI_TRANSACTIONS' CREATED WITH CDC ENABLED...
2025-05-24T13:35:51.962+0000: [GC (Allocation Failure) [PSYoungGen: 1426309K->13037K(1512960K)] 1632457K->219193K(4774912K), 0.0222959 secs] [Times: user=0.04 sys=0.00, real=0.02 secs] 
Read Stream Started.........
2025-05-24T13:42:11.350+0000: [GC (Allocation Failure) [PSYoungGen: 1413191K->24242K(1515520K)] 1619346K->230398K(4777472K), 0.0286147 secs] [Times: user=0.05 sys=0.00, real=0.03 secs] 
Processing batch: 0
2025-05-24T13:42:17.397+0000: [GC (Allocation Failure) [PSYoungGen: 1424562K->38591K(1520640K)] 1630718K->244747K(4782592K), 0.0689670 secs] [Times: user=0.11 sys=0.00, real=0.07 secs] 
2025-05-24T13:42:29.187+0000: [GC (Allocation Failure) [PSYoungGen: 1445055K->40927K(1516544K)] 1651211K->247083K(4778496K), 0.0547757 secs] [Times: user=0.08 sys=0.00, real=0.06 secs] 
Batch processed successfully.
Processing batch: 1
2025-05-24T13:42:34.844+0000: [GC (Allocation Failure) [PSYoungGen: 1447391K->49288K(1530880K)] 1653547K->255443K(4792832K), 0.0488370 secs] [Times: user=0.09 sys=0.01, real=0.05 secs] 
2025-05-24T13:44:02.713+0000: [GC (Allocation Failure) [PSYoungGen: 1474696K->46432K(1525248K)] 1680851K->252596K(4787200K), 0.1448888 secs] [Times: user=0.12 sys=0.00, real=0.14 secs] 
2025-05-24T13:44:08.699+0000: [GC (Allocation Failure) [PSYoungGen: 1471840K->54388K(1538048K)] 1678004K->260552K(4800000K), 0.0628547 secs] [Times: user=0.10 sys=0.00, real=0.07 secs] 
Batch processed successfully.
Processing batch: 2
2025-05-24T13:44:13.799+0000: [GC (Allocation Failure) [PSYoungGen: 1496552K->92647K(1535488K)] 1702715K->341649K(4797440K), 0.0778284 secs] [Times: user=0.13 sys=0.00, real=0.07 secs] 
2025-05-24T13:44:18.264+0000: [GC (Allocation Failure) [PSYoungGen: 1535463K->95225K(1401344K)] 1784465K->436508K(4663296K), 0.0676124 secs] [Times: user=0.12 sys=0.00, real=0.07 secs] 
2025-05-24T13:44:22.555+0000: [GC (Allocation Failure) [PSYoungGen: 1401337K->113381K(1419776K)] 1742620K->454672K(4681728K), 0.0666404 secs] [Times: user=0.11 sys=0.00, real=0.07 secs] 
Processing batch: 3
2025-05-24T13:44:27.273+0000: [GC (Allocation Failure) [PSYoungGen: 1419493K->120308K(1446912K)] 1760784K->461599K(4708864K), 0.0622291 secs] [Times: user=0.12 sys=0.00, real=0.06 secs] 
2025-05-24T13:44:42.385+0000: [GC (Allocation Failure) [PSYoungGen: 1398772K->119534K(1398272K)] 1740063K->460825K(4660224K), 0.0587070 secs] [Times: user=0.10 sys=0.00, real=0.06 secs] 
2025-05-24T13:44:48.350+0000: [GC (Allocation Failure) [PSYoungGen: 1397998K->127301K(1437184K)] 1739289K->534128K(4699136K), 0.1212193 secs] [Times: user=0.16 sys=0.03, real=0.12 secs] 
Batch processed successfully.
Processing batch: 4
2025-05-24T13:44:53.156+0000: [GC (Allocation Failure) [PSYoungGen: 1383237K->135326K(1391616K)] 1790064K->542153K(4653568K), 0.0715512 secs] [Times: user=0.12 sys=0.00, real=0.07 secs] 
2025-05-24T13:44:57.649+0000: [GC (Allocation Failure) [PSYoungGen: 1391262K->195052K(1370112K)] 1798089K->615188K(4632064K), 0.1347674 secs] [Times: user=0.15 sys=0.01, real=0.14 secs] 
2025-05-24T13:45:01.492+0000: [GC (Allocation Failure) [PSYoungGen: 1370092K->133950K(1402880K)] 1790228K->557450K(4664832K), 0.0757698 secs] [Times: user=0.14 sys=0.00, real=0.07 secs] 
2025-05-24T13:45:05.235+0000: [GC (Allocation Failure) [PSYoungGen: 1308990K->142350K(1402368K)] 1732490K->565858K(4664320K), 0.0792010 secs] [Times: user=0.14 sys=0.00, real=0.08 secs] 
Processing batch: 5
2025-05-24T13:45:09.889+0000: [GC (Allocation Failure) [PSYoungGen: 1318414K->151883K(1328128K)] 1741922K->575806K(4590080K), 0.0913682 secs] [Times: user=0.16 sys=0.00, real=0.10 secs] 
2025-05-24T13:45:44.053+0000: [GC (Allocation Failure) [PSYoungGen: 1327947K->205549K(1355776K)] 1751870K->630859K(4617728K), 0.0786017 secs] [Times: user=0.14 sys=0.00, real=0.08 secs] 


<img width="1315" alt="image" src="https://github.com/user-attachments/assets/579a50a7-778d-420f-8666-7ec3087fa055" />

