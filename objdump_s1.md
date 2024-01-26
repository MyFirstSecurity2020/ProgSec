# 
```c
[XD] % objdump -S -M intel -j .text  add2

add2:     file format elf64-x86-64


Disassembly of section .text:

0000000000000540 <_start>:
 540:	31 ed                	xor    ebp,ebp
 542:	49 89 d1             	mov    r9,rdx
 545:	5e                   	pop    rsi
 546:	48 89 e2             	mov    rdx,rsp
 549:	48 83 e4 f0          	and    rsp,0xfffffffffffffff0
 54d:	50                   	push   rax
 54e:	54                   	push   rsp
 54f:	4c 8d 05 ca 01 00 00 	lea    r8,[rip+0x1ca]        # 720 <__libc_csu_fini>
 556:	48 8d 0d 53 01 00 00 	lea    rcx,[rip+0x153]        # 6b0 <__libc_csu_init>
 55d:	48 8d 3d 08 01 00 00 	lea    rdi,[rip+0x108]        # 66c <main>
 564:	ff 15 76 0a 20 00    	call   QWORD PTR [rip+0x200a76]        # 200fe0 <__libc_start_main@GLIBC_2.2.5>
 56a:	f4                   	hlt    
 56b:	0f 1f 44 00 00       	nop    DWORD PTR [rax+rax*1+0x0]

0000000000000570 <deregister_tm_clones>:
 570:	48 8d 3d 99 0a 20 00 	lea    rdi,[rip+0x200a99]        # 201010 <__TMC_END__>
 577:	55                   	push   rbp
 578:	48 8d 05 91 0a 20 00 	lea    rax,[rip+0x200a91]        # 201010 <__TMC_END__>
 57f:	48 39 f8             	cmp    rax,rdi
 582:	48 89 e5             	mov    rbp,rsp
 585:	74 19                	je     5a0 <deregister_tm_clones+0x30>
 587:	48 8b 05 4a 0a 20 00 	mov    rax,QWORD PTR [rip+0x200a4a]        # 200fd8 <_ITM_deregisterTMCloneTable>
 58e:	48 85 c0             	test   rax,rax
 591:	74 0d                	je     5a0 <deregister_tm_clones+0x30>
 593:	5d                   	pop    rbp
 594:	ff e0                	jmp    rax
 596:	66 2e 0f 1f 84 00 00 	nop    WORD PTR cs:[rax+rax*1+0x0]
 59d:	00 00 00 
 5a0:	5d                   	pop    rbp
 5a1:	c3                   	ret    
 5a2:	0f 1f 40 00          	nop    DWORD PTR [rax+0x0]
 5a6:	66 2e 0f 1f 84 00 00 	nop    WORD PTR cs:[rax+rax*1+0x0]
 5ad:	00 00 00 

00000000000005b0 <register_tm_clones>:
 5b0:	48 8d 3d 59 0a 20 00 	lea    rdi,[rip+0x200a59]        # 201010 <__TMC_END__>
 5b7:	48 8d 35 52 0a 20 00 	lea    rsi,[rip+0x200a52]        # 201010 <__TMC_END__>
 5be:	55                   	push   rbp
 5bf:	48 29 fe             	sub    rsi,rdi
 5c2:	48 89 e5             	mov    rbp,rsp
 5c5:	48 c1 fe 03          	sar    rsi,0x3
 5c9:	48 89 f0             	mov    rax,rsi
 5cc:	48 c1 e8 3f          	shr    rax,0x3f
 5d0:	48 01 c6             	add    rsi,rax
 5d3:	48 d1 fe             	sar    rsi,1
 5d6:	74 18                	je     5f0 <register_tm_clones+0x40>
 5d8:	48 8b 05 11 0a 20 00 	mov    rax,QWORD PTR [rip+0x200a11]        # 200ff0 <_ITM_registerTMCloneTable>
 5df:	48 85 c0             	test   rax,rax
 5e2:	74 0c                	je     5f0 <register_tm_clones+0x40>
 5e4:	5d                   	pop    rbp
 5e5:	ff e0                	jmp    rax
 5e7:	66 0f 1f 84 00 00 00 	nop    WORD PTR [rax+rax*1+0x0]
 5ee:	00 00 
 5f0:	5d                   	pop    rbp
 5f1:	c3                   	ret    
 5f2:	0f 1f 40 00          	nop    DWORD PTR [rax+0x0]
 5f6:	66 2e 0f 1f 84 00 00 	nop    WORD PTR cs:[rax+rax*1+0x0]
 5fd:	00 00 00 

0000000000000600 <__do_global_dtors_aux>:
 600:	80 3d 09 0a 20 00 00 	cmp    BYTE PTR [rip+0x200a09],0x0        # 201010 <__TMC_END__>
 607:	75 2f                	jne    638 <__do_global_dtors_aux+0x38>
 609:	48 83 3d e7 09 20 00 	cmp    QWORD PTR [rip+0x2009e7],0x0        # 200ff8 <__cxa_finalize@GLIBC_2.2.5>
 610:	00 
 611:	55                   	push   rbp
 612:	48 89 e5             	mov    rbp,rsp
 615:	74 0c                	je     623 <__do_global_dtors_aux+0x23>
 617:	48 8b 3d ea 09 20 00 	mov    rdi,QWORD PTR [rip+0x2009ea]        # 201008 <__dso_handle>
 61e:	e8 0d ff ff ff       	call   530 <__cxa_finalize@plt>
 623:	e8 48 ff ff ff       	call   570 <deregister_tm_clones>
 628:	c6 05 e1 09 20 00 01 	mov    BYTE PTR [rip+0x2009e1],0x1        # 201010 <__TMC_END__>
 62f:	5d                   	pop    rbp
 630:	c3                   	ret    
 631:	0f 1f 80 00 00 00 00 	nop    DWORD PTR [rax+0x0]
 638:	f3 c3                	repz ret 
 63a:	66 0f 1f 44 00 00    	nop    WORD PTR [rax+rax*1+0x0]

0000000000000640 <frame_dummy>:
 640:	55                   	push   rbp
 641:	48 89 e5             	mov    rbp,rsp
 644:	5d                   	pop    rbp
 645:	e9 66 ff ff ff       	jmp    5b0 <register_tm_clones>

000000000000064a <add>:
#include <stdio.h>

int add(int x, int y)
{
 64a:	55                   	push   rbp
 64b:	48 89 e5             	mov    rbp,rsp
 64e:	89 7d ec             	mov    DWORD PTR [rbp-0x14],edi
 651:	89 75 e8             	mov    DWORD PTR [rbp-0x18],esi
  int sum = 0;
 654:	c7 45 fc 00 00 00 00 	mov    DWORD PTR [rbp-0x4],0x0
  sum += x;
 65b:	8b 45 ec             	mov    eax,DWORD PTR [rbp-0x14]
 65e:	01 45 fc             	add    DWORD PTR [rbp-0x4],eax
  sum += y;
 661:	8b 45 e8             	mov    eax,DWORD PTR [rbp-0x18]
 664:	01 45 fc             	add    DWORD PTR [rbp-0x4],eax
  return sum;
 667:	8b 45 fc             	mov    eax,DWORD PTR [rbp-0x4]
}
 66a:	5d                   	pop    rbp
 66b:	c3                   	ret    

000000000000066c <main>:

int main()
{
 66c:	55                   	push   rbp
 66d:	48 89 e5             	mov    rbp,rsp
 670:	48 83 ec 10          	sub    rsp,0x10
  int a = 2, b = 3;
 674:	c7 45 f8 02 00 00 00 	mov    DWORD PTR [rbp-0x8],0x2
 67b:	c7 45 fc 03 00 00 00 	mov    DWORD PTR [rbp-0x4],0x3
  printf("%d\n",add(a, b) );
 682:	8b 55 fc             	mov    edx,DWORD PTR [rbp-0x4]
 685:	8b 45 f8             	mov    eax,DWORD PTR [rbp-0x8]
 688:	89 d6                	mov    esi,edx
 68a:	89 c7                	mov    edi,eax
 68c:	e8 b9 ff ff ff       	call   64a <add>
 691:	89 c6                	mov    esi,eax
 693:	48 8d 3d 9a 00 00 00 	lea    rdi,[rip+0x9a]        # 734 <_IO_stdin_used+0x4>
 69a:	b8 00 00 00 00       	mov    eax,0x0
 69f:	e8 7c fe ff ff       	call   520 <printf@plt>
  return 0;
 6a4:	b8 00 00 00 00       	mov    eax,0x0
}
 6a9:	c9                   	leave  
 6aa:	c3                   	ret    
 6ab:	0f 1f 44 00 00       	nop    DWORD PTR [rax+rax*1+0x0]

00000000000006b0 <__libc_csu_init>:
 6b0:	41 57                	push   r15
 6b2:	41 56                	push   r14
 6b4:	49 89 d7             	mov    r15,rdx
 6b7:	41 55                	push   r13
 6b9:	41 54                	push   r12
 6bb:	4c 8d 25 f6 06 20 00 	lea    r12,[rip+0x2006f6]        # 200db8 <__frame_dummy_init_array_entry>
 6c2:	55                   	push   rbp
 6c3:	48 8d 2d f6 06 20 00 	lea    rbp,[rip+0x2006f6]        # 200dc0 <__init_array_end>
 6ca:	53                   	push   rbx
 6cb:	41 89 fd             	mov    r13d,edi
 6ce:	49 89 f6             	mov    r14,rsi
 6d1:	4c 29 e5             	sub    rbp,r12
 6d4:	48 83 ec 08          	sub    rsp,0x8
 6d8:	48 c1 fd 03          	sar    rbp,0x3
 6dc:	e8 0f fe ff ff       	call   4f0 <_init>
 6e1:	48 85 ed             	test   rbp,rbp
 6e4:	74 20                	je     706 <__libc_csu_init+0x56>
 6e6:	31 db                	xor    ebx,ebx
 6e8:	0f 1f 84 00 00 00 00 	nop    DWORD PTR [rax+rax*1+0x0]
 6ef:	00 
 6f0:	4c 89 fa             	mov    rdx,r15
 6f3:	4c 89 f6             	mov    rsi,r14
 6f6:	44 89 ef             	mov    edi,r13d
 6f9:	41 ff 14 dc          	call   QWORD PTR [r12+rbx*8]
 6fd:	48 83 c3 01          	add    rbx,0x1
 701:	48 39 dd             	cmp    rbp,rbx
 704:	75 ea                	jne    6f0 <__libc_csu_init+0x40>
 706:	48 83 c4 08          	add    rsp,0x8
 70a:	5b                   	pop    rbx
 70b:	5d                   	pop    rbp
 70c:	41 5c                	pop    r12
 70e:	41 5d                	pop    r13
 710:	41 5e                	pop    r14
 712:	41 5f                	pop    r15
 714:	c3                   	ret    
 715:	90                   	nop
 716:	66 2e 0f 1f 84 00 00 	nop    WORD PTR cs:[rax+rax*1+0x0]
 71d:	00 00 00 

0000000000000720 <__libc_csu_fini>:
 720:	f3 c3                	repz ret 

```
