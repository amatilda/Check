# Check
Check

MallocStackLogging

If set, malloc remembers the function call stack at the time of each allocation.

MallocStackLoggingNoCompact

This option is similar to MallocStackLogging but makes sure that all allocations are logged, no matter how small or how short lived the buffer may be.

MallocScribble

If set, free sets each byte of every released block to the value 0x55.

MallocPreScribble

If set, malloc sets each byte of a newly allocated block to the value 0xAA. This increases the likelihood that a program making assumptions about freshly allocated memory fails.

MallocGuardEdges

If set, malloc adds guard pages before and after large allocations.

MallocDoNotProtectPrelude

Fine-grain control over the behavior of MallocGuardEdges: If set, malloc does not place a guard page at the head of each large block allocation.

MallocDoNotProtectPostlude

Fine-grain control over the behavior of MallocGuardEdges: If set, malloc does not place a guard page at the tail of each large block allocation.

MallocCheckHeapStart

Set this variable to the number of allocations before malloc will begin validating the heap. If not set, malloc does not validate the heap.

MallocCheckHeapEach

Set this variable to the number of allocations before malloc should validate the heap. If not set, malloc does not validate the heap.

objdump -lazy-bind 

	FILE *file1;
	file1 = fopen("/Users/amatilda/Subject/42sh/test.txt", "a");
	fprintf(file1, "%s\n","test\n");
	fclose(file1);
  
 void	*ft_malloc(register size_t n)
{
	register void		*out;

	if ((out = malloc(n)) == 0)
		return (0);
	return (out);
}

void	ft_free(register void *buff)
{
	free(buff);
}

t_main_42sh			*g_lp_array;

extern t_main_42sh			*g_lp_array;

https://developer.apple.com/library/archive/documentation/Performance/Conceptual/ManagingMemory/Articles/FindingPatterns.html#//apple_ref/doc/uid/20001882-CJBJFIDD

https://cdn.intra.42.fr/pdf/pdf/960/norme.en.pdf
