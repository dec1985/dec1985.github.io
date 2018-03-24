# 研究优化feeds pool内存使用方法，最终确定使用namedtuple方案。 

单纯的对比namedtuple和dict，差不多能节约90%的内存使用量。 

其它备选方案包括：sqlit3/shelve/mmap/python3.6/blist.sorteddict/pyjudy/pre-fork worker pool/pypy-stm等，都因为各种原因（不靠谱、技术不成熟、工作量非常大）等放弃。 最终实施工期预计在3天左右，预计完成noti之后马上开工。 

refs: http://fred18:8848/munin/fp1/fp1/memory.html
