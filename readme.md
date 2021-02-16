## bug1

/mockcpp/include/mockcpp/PageAllocator.h:37:25: error: cast from ‘void*’ to ‘int’ loses precision [-fpermissive]
   return (void *)(((int)addr) & ~(pageSize() - 1));

修改：
	win32	win64	linux32	linux64
int 	4	4	4	4
long	4	4	4	8

![图 1](images/5b0a256da7ff8920f64735509c8d63f8b192838382de8f24520f12c669acf44b.png)  
