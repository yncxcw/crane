This is evaluation framework of m-smr system!
Run:
	./eval.py *.cfg

Results (last updated on 11/27/2014):
	[Server=Mongoose, Server count=3, Client=Ab, Client count=100]
	With proxy:
		System:
			Consensus Time(5434):
				mean: 11784.3829405 us
				std: 12637.0019955
			Response Time(5434):  
				mean: 12137.4390869 us
				std: 12670.9796392
			Throughput: 1125.57004518 Req/s
		Real Server:
			Time per request: 6024 us
			Requests per second: 1660.03
	Without proxy:
		Time per request: 1865 us
		Requests per second: 5361.93 Req/s

	[Server=Apache, Server count=3, Client=Ab, Client count=100]
	With proxy:
		System:
			Consensus Time(5577): 
				mean: 10093.2689001 us
				std: 15218.2857854
			Response Time(5577):
				mean: 10359.6252461 us
				std: 15281.7748126
			Throughput: 1963.44173126 Req/s
		Real Server:
			Time per request: 7110 us
			Requests per second: 1406.47
	Without proxy:
		Time per request: 17985 us
		Requests per second: 556.02 Req/s

	[Server=Lighttpd, Server count=3, Client=Ab, Client count=100]
	With proxy:
		System:
			Concensus Time(4799):
				mean: 8588.36478158 us
				std: 12737.463843
			Response Time(4799): 
				mean: 8869.2045171 us
				std: 12776.5457869
			Throughput: 776.35067849 Req/s
		Real Server:
			Time per request: 37253 us
			Requests per second: 268.43
	Without proxy:
		Time per request: 26864 us
		Requests per second: 372.25 Req/s

	[Server=Pgsql, Server count=3, Client=pgbench, Client count=2]
	With proxy:
		System:
			Consensus Time(28176): 
				mean: 886.624785799 us
				std: 6457.45645969
			Response Time(28176):
				mean: 991.669019673 us
				std: 6524.97343144
			Throughput: 262.586008948 Req/s
		Real Server:
			tps: 49.670571
	Without proxy:
		tps: 107.301376

	[Server=Ssdb, Server count=3, Client=ssdb-bench, Client count=100]
	With proxy:
		System:
			Consensus Time(120000): 
				mean: 20339.3639863 us
				std: 21865.9739571
			Response Time(120000): 
				mean: 20759.1385961 us
				std: 22028.4780573
			Throughput: 1954.05336637 Req/s
		Real Server(set):
			qps: 1214
			time: 82000 us
	Without proxy:
		qps: 30564
		time: 3000 us

	[Server=Mongodb, Server count=3, Client=ycsb, Client count=2]
	With proxy:
		System:
			Consensus Time(17021): 
				mean: 27936.6877474 us
				std: 101034.193019
			Response Time(17021):
				mean: 28657.3323245 us
				std: 101076.672629
			Throughput: 198.860874368 Req/s
		Real Server:
			AverageLatency: 193439 us
			Throughput: 11.807351256892542
	Without proxy:
		Average Latency: 7236.46511627907 us
		Throughput: 2801.1204481792715 Req/s

	[Server=proftpd, Server count=3, Client=dkftpbench, Client Count=10]
	With Proxy:
		System:
			Concensus Time(2600):
				mean: 661.111519887 us
				std: 3415.66346119
			Response Time(2600):
				mean: 703.23247176 us
				std: 3422.55397882
			Throughput: 25.1892199412 Req/s
		Real server:
			3579 bytes per second
	Without Proxy:
		3584 bytes per second

	[Server=memcached, Server Count=3, Client=memslap, Client Count=100]
	With Proxy:
		System:
			Concensus Time(13043):
				mean: 2582.75371821 us
				std: 2813.53107613
			Response Time(13043):
				mean: 2873.49056103 us
				std: 2950.63957846
			Throughput: 2020.00553691 Req/s
		Real server:
			Loading time: 47000 us
	Without Proxy:
		Loading time: 8000 us

	[Server=mysql]
	(to be done)
	
	[Server=ldap]
	(to be done)
