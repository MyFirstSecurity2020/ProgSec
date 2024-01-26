## objdump -S -j .text -M intel helloCTFer --no-show-raw-insn
- 不顯示機器指令 ==> --no-show-raw-insn
```c


helloCTFer:     file format elf64-x86-64

Disassembly of section .text:

0000000000000530 <_start>:
 530:	xor    ebp,ebp
 532:	mov    r9,rdx
 535:	pop    rsi
 536:	mov    rdx,rsp
 539:	and    rsp,0xfffffffffffffff0
 53d:	push   rax
 53e:	push   rsp
 53f:	lea    r8,[rip+0x18a]        # 6d0 <__libc_csu_fini>
 546:	lea    rcx,[rip+0x113]        # 660 <__libc_csu_init>
 54d:	lea    rdi,[rip+0xe6]        # 63a <main>
 554:	call   QWORD PTR [rip+0x200a86]        # 200fe0 <__libc_start_main@GLIBC_2.2.5>
 55a:	hlt    
 55b:	nop    DWORD PTR [rax+rax*1+0x0]

0000000000000560 <deregister_tm_clones>:
 560:	lea    rdi,[rip+0x200aa9]        # 201010 <__TMC_END__>
 567:	push   rbp
 568:	lea    rax,[rip+0x200aa1]        # 201010 <__TMC_END__>
 56f:	cmp    rax,rdi
 572:	mov    rbp,rsp
 575:	je     590 <deregister_tm_clones+0x30>
 577:	mov    rax,QWORD PTR [rip+0x200a5a]        # 200fd8 <_ITM_deregisterTMCloneTable>
 57e:	test   rax,rax
 581:	je     590 <deregister_tm_clones+0x30>
 583:	pop    rbp
 584:	jmp    rax
 586:	nop    WORD PTR cs:[rax+rax*1+0x0]
 590:	pop    rbp
 591:	ret    
 592:	nop    DWORD PTR [rax+0x0]
 596:	nop    WORD PTR cs:[rax+rax*1+0x0]

00000000000005a0 <register_tm_clones>:
 5a0:	lea    rdi,[rip+0x200a69]        # 201010 <__TMC_END__>
 5a7:	lea    rsi,[rip+0x200a62]        # 201010 <__TMC_END__>
 5ae:	push   rbp
 5af:	sub    rsi,rdi
 5b2:	mov    rbp,rsp
 5b5:	sar    rsi,0x3
 5b9:	mov    rax,rsi
 5bc:	shr    rax,0x3f
 5c0:	add    rsi,rax
 5c3:	sar    rsi,1
 5c6:	je     5e0 <register_tm_clones+0x40>
 5c8:	mov    rax,QWORD PTR [rip+0x200a21]        # 200ff0 <_ITM_registerTMCloneTable>
 5cf:	test   rax,rax
 5d2:	je     5e0 <register_tm_clones+0x40>
 5d4:	pop    rbp
 5d5:	jmp    rax
 5d7:	nop    WORD PTR [rax+rax*1+0x0]
 5e0:	pop    rbp
 5e1:	ret    
 5e2:	nop    DWORD PTR [rax+0x0]
 5e6:	nop    WORD PTR cs:[rax+rax*1+0x0]

00000000000005f0 <__do_global_dtors_aux>:
 5f0:	cmp    BYTE PTR [rip+0x200a19],0x0        # 201010 <__TMC_END__>
 5f7:	jne    628 <__do_global_dtors_aux+0x38>
 5f9:	cmp    QWORD PTR [rip+0x2009f7],0x0        # 200ff8 <__cxa_finalize@GLIBC_2.2.5>
 601:	push   rbp
 602:	mov    rbp,rsp
 605:	je     613 <__do_global_dtors_aux+0x23>
 607:	mov    rdi,QWORD PTR [rip+0x2009fa]        # 201008 <__dso_handle>
 60e:	call   520 <__cxa_finalize@plt>
 613:	call   560 <deregister_tm_clones>
 618:	mov    BYTE PTR [rip+0x2009f1],0x1        # 201010 <__TMC_END__>
 61f:	pop    rbp
 620:	ret    
 621:	nop    DWORD PTR [rax+0x0]
 628:	repz ret 
 62a:	nop    WORD PTR [rax+rax*1+0x0]

0000000000000630 <frame_dummy>:
 630:	push   rbp
 631:	mov    rbp,rsp
 634:	pop    rbp
 635:	jmp    5a0 <register_tm_clones>

000000000000063a <main>:
#include <stdio.h>

int main()
{
 63a:	push   rbp
 63b:	mov    rbp,rsp
   printf("Hello CTFer\n");
 63e:	lea    rdi,[rip+0x9f]        # 6e4 <_IO_stdin_used+0x4>
 645:	call   510 <puts@plt>
   return 0;
 64a:	mov    eax,0x0
}
 64f:	pop    rbp
 650:	ret    
 651:	nop    WORD PTR cs:[rax+rax*1+0x0]
 65b:	nop    DWORD PTR [rax+rax*1+0x0]

0000000000000660 <__libc_csu_init>:
 660:	push   r15
 662:	push   r14
 664:	mov    r15,rdx
 667:	push   r13
 669:	push   r12
 66b:	lea    r12,[rip+0x200746]        # 200db8 <__frame_dummy_init_array_entry>
 672:	push   rbp
 673:	lea    rbp,[rip+0x200746]        # 200dc0 <__init_array_end>
 67a:	push   rbx
 67b:	mov    r13d,edi
 67e:	mov    r14,rsi
 681:	sub    rbp,r12
 684:	sub    rsp,0x8
 688:	sar    rbp,0x3
 68c:	call   4e8 <_init>
 691:	test   rbp,rbp
 694:	je     6b6 <__libc_csu_init+0x56>
 696:	xor    ebx,ebx
 698:	nop    DWORD PTR [rax+rax*1+0x0]
 6a0:	mov    rdx,r15
 6a3:	mov    rsi,r14
 6a6:	mov    edi,r13d
 6a9:	call   QWORD PTR [r12+rbx*8]
 6ad:	add    rbx,0x1
 6b1:	cmp    rbp,rbx
 6b4:	jne    6a0 <__libc_csu_init+0x40>
 6b6:	add    rsp,0x8
 6ba:	pop    rbx
 6bb:	pop    rbp
 6bc:	pop    r12
 6be:	pop    r13
 6c0:	pop    r14
 6c2:	pop    r15
 6c4:	ret    
 6c5:	nop
 6c6:	nop    WORD PTR cs:[rax+rax*1+0x0]

00000000000006d0 <__libc_csu_fini>:
 6d0:	repz ret 


```
