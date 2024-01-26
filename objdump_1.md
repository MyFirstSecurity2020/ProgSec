##

```c

add2:     file format elf64-x86-64


Disassembly of section .interp:

0000000000000238 <.interp>:
 238:	2f                   	(bad)  
 239:	6c                   	ins    BYTE PTR es:[rdi],dx
 23a:	69 62 36 34 2f 6c 64 	imul   esp,DWORD PTR [rdx+0x36],0x646c2f34
 241:	2d 6c 69 6e 75       	sub    eax,0x756e696c
 246:	78 2d                	js     275 <_init-0x27b>
 248:	78 38                	js     282 <_init-0x26e>
 24a:	36 2d 36 34 2e 73    	ss sub eax,0x732e3436
 250:	6f                   	outs   dx,DWORD PTR ds:[rsi]
 251:	2e 32 00             	xor    al,BYTE PTR cs:[rax]

Disassembly of section .note.ABI-tag:

0000000000000254 <.note.ABI-tag>:
 254:	04 00                	add    al,0x0
 256:	00 00                	add    BYTE PTR [rax],al
 258:	10 00                	adc    BYTE PTR [rax],al
 25a:	00 00                	add    BYTE PTR [rax],al
 25c:	01 00                	add    DWORD PTR [rax],eax
 25e:	00 00                	add    BYTE PTR [rax],al
 260:	47                   	rex.RXB
 261:	4e 55                	rex.WRX push rbp
 263:	00 00                	add    BYTE PTR [rax],al
 265:	00 00                	add    BYTE PTR [rax],al
 267:	00 03                	add    BYTE PTR [rbx],al
 269:	00 00                	add    BYTE PTR [rax],al
 26b:	00 02                	add    BYTE PTR [rdx],al
 26d:	00 00                	add    BYTE PTR [rax],al
 26f:	00 00                	add    BYTE PTR [rax],al
 271:	00 00                	add    BYTE PTR [rax],al
	...

Disassembly of section .note.gnu.build-id:

0000000000000274 <.note.gnu.build-id>:
 274:	04 00                	add    al,0x0
 276:	00 00                	add    BYTE PTR [rax],al
 278:	14 00                	adc    al,0x0
 27a:	00 00                	add    BYTE PTR [rax],al
 27c:	03 00                	add    eax,DWORD PTR [rax]
 27e:	00 00                	add    BYTE PTR [rax],al
 280:	47                   	rex.RXB
 281:	4e 55                	rex.WRX push rbp
 283:	00 78 ea             	add    BYTE PTR [rax-0x16],bh
 286:	19 3a                	sbb    DWORD PTR [rdx],edi
 288:	12 b9 d1 60 5f db    	adc    bh,BYTE PTR [rcx-0x24a09f2f]
 28e:	e1 c8                	loope  258 <_init-0x298>
 290:	34 a7                	xor    al,0xa7
 292:	3b 51 f4             	cmp    edx,DWORD PTR [rcx-0xc]
 295:	48 88 03             	rex.W mov BYTE PTR [rbx],al

Disassembly of section .gnu.hash:

0000000000000298 <.gnu.hash>:
 298:	01 00                	add    DWORD PTR [rax],eax
 29a:	00 00                	add    BYTE PTR [rax],al
 29c:	01 00                	add    DWORD PTR [rax],eax
 29e:	00 00                	add    BYTE PTR [rax],al
 2a0:	01 00                	add    DWORD PTR [rax],eax
	...

Disassembly of section .dynsym:

00000000000002b8 <.dynsym>:
	...
 2d0:	3f                   	(bad)  
 2d1:	00 00                	add    BYTE PTR [rax],al
 2d3:	00 20                	add    BYTE PTR [rax],ah
	...
 2e5:	00 00                	add    BYTE PTR [rax],al
 2e7:	00 0b                	add    BYTE PTR [rbx],cl
 2e9:	00 00                	add    BYTE PTR [rax],al
 2eb:	00 12                	add    BYTE PTR [rdx],dl
	...
 2fd:	00 00                	add    BYTE PTR [rax],al
 2ff:	00 21                	add    BYTE PTR [rcx],ah
 301:	00 00                	add    BYTE PTR [rax],al
 303:	00 12                	add    BYTE PTR [rdx],dl
	...
 315:	00 00                	add    BYTE PTR [rax],al
 317:	00 5b 00             	add    BYTE PTR [rbx+0x0],bl
 31a:	00 00                	add    BYTE PTR [rax],al
 31c:	20 00                	and    BYTE PTR [rax],al
	...
 32e:	00 00                	add    BYTE PTR [rax],al
 330:	6a 00                	push   0x0
 332:	00 00                	add    BYTE PTR [rax],al
 334:	20 00                	and    BYTE PTR [rax],al
	...
 346:	00 00                	add    BYTE PTR [rax],al
 348:	12 00                	adc    al,BYTE PTR [rax]
 34a:	00 00                	add    BYTE PTR [rax],al
 34c:	22 00                	and    al,BYTE PTR [rax]
	...

Disassembly of section .dynstr:

0000000000000360 <.dynstr>:
 360:	00 6c 69 62          	add    BYTE PTR [rcx+rbp*2+0x62],ch
 364:	63 2e                	movsxd ebp,DWORD PTR [rsi]
 366:	73 6f                	jae    3d7 <_init-0x119>
 368:	2e 36 00 70 72       	cs add BYTE PTR ss:[rax+0x72],dh
 36d:	69 6e 74 66 00 5f 5f 	imul   ebp,DWORD PTR [rsi+0x74],0x5f5f0066
 374:	63 78 61             	movsxd edi,DWORD PTR [rax+0x61]
 377:	5f                   	pop    rdi
 378:	66 69 6e 61 6c 69    	imul   bp,WORD PTR [rsi+0x61],0x696c
 37e:	7a 65                	jp     3e5 <_init-0x10b>
 380:	00 5f 5f             	add    BYTE PTR [rdi+0x5f],bl
 383:	6c                   	ins    BYTE PTR es:[rdi],dx
 384:	69 62 63 5f 73 74 61 	imul   esp,DWORD PTR [rdx+0x63],0x6174735f
 38b:	72 74                	jb     401 <_init-0xef>
 38d:	5f                   	pop    rdi
 38e:	6d                   	ins    DWORD PTR es:[rdi],dx
 38f:	61                   	(bad)  
 390:	69 6e 00 47 4c 49 42 	imul   ebp,DWORD PTR [rsi+0x0],0x42494c47
 397:	43 5f                	rex.XB pop r15
 399:	32 2e                	xor    ch,BYTE PTR [rsi]
 39b:	32 2e                	xor    ch,BYTE PTR [rsi]
 39d:	35 00 5f 49 54       	xor    eax,0x54495f00
 3a2:	4d 5f                	rex.WRB pop r15
 3a4:	64 65 72 65          	fs gs jb 40d <_init-0xe3>
 3a8:	67 69 73 74 65 72 54 	imul   esi,DWORD PTR [ebx+0x74],0x4d547265
 3af:	4d 
 3b0:	43 6c                	rex.XB ins BYTE PTR es:[rdi],dx
 3b2:	6f                   	outs   dx,DWORD PTR ds:[rsi]
 3b3:	6e                   	outs   dx,BYTE PTR ds:[rsi]
 3b4:	65 54                	gs push rsp
 3b6:	61                   	(bad)  
 3b7:	62                   	(bad)  
 3b8:	6c                   	ins    BYTE PTR es:[rdi],dx
 3b9:	65 00 5f 5f          	add    BYTE PTR gs:[rdi+0x5f],bl
 3bd:	67 6d                	ins    DWORD PTR es:[edi],dx
 3bf:	6f                   	outs   dx,DWORD PTR ds:[rsi]
 3c0:	6e                   	outs   dx,BYTE PTR ds:[rsi]
 3c1:	5f                   	pop    rdi
 3c2:	73 74                	jae    438 <_init-0xb8>
 3c4:	61                   	(bad)  
 3c5:	72 74                	jb     43b <_init-0xb5>
 3c7:	5f                   	pop    rdi
 3c8:	5f                   	pop    rdi
 3c9:	00 5f 49             	add    BYTE PTR [rdi+0x49],bl
 3cc:	54                   	push   rsp
 3cd:	4d 5f                	rex.WRB pop r15
 3cf:	72 65                	jb     436 <_init-0xba>
 3d1:	67 69 73 74 65 72 54 	imul   esi,DWORD PTR [ebx+0x74],0x4d547265
 3d8:	4d 
 3d9:	43 6c                	rex.XB ins BYTE PTR es:[rdi],dx
 3db:	6f                   	outs   dx,DWORD PTR ds:[rsi]
 3dc:	6e                   	outs   dx,BYTE PTR ds:[rsi]
 3dd:	65 54                	gs push rsp
 3df:	61                   	(bad)  
 3e0:	62                   	.byte 0x62
 3e1:	6c                   	ins    BYTE PTR es:[rdi],dx
 3e2:	65                   	gs
	...

Disassembly of section .gnu.version:

00000000000003e4 <.gnu.version>:
 3e4:	00 00                	add    BYTE PTR [rax],al
 3e6:	00 00                	add    BYTE PTR [rax],al
 3e8:	02 00                	add    al,BYTE PTR [rax]
 3ea:	02 00                	add    al,BYTE PTR [rax]
 3ec:	00 00                	add    BYTE PTR [rax],al
 3ee:	00 00                	add    BYTE PTR [rax],al
 3f0:	02 00                	add    al,BYTE PTR [rax]

Disassembly of section .gnu.version_r:

00000000000003f8 <.gnu.version_r>:
 3f8:	01 00                	add    DWORD PTR [rax],eax
 3fa:	01 00                	add    DWORD PTR [rax],eax
 3fc:	01 00                	add    DWORD PTR [rax],eax
 3fe:	00 00                	add    BYTE PTR [rax],al
 400:	10 00                	adc    BYTE PTR [rax],al
 402:	00 00                	add    BYTE PTR [rax],al
 404:	00 00                	add    BYTE PTR [rax],al
 406:	00 00                	add    BYTE PTR [rax],al
 408:	75 1a                	jne    424 <_init-0xcc>
 40a:	69 09 00 00 02 00    	imul   ecx,DWORD PTR [rcx],0x20000
 410:	33 00                	xor    eax,DWORD PTR [rax]
 412:	00 00                	add    BYTE PTR [rax],al
 414:	00 00                	add    BYTE PTR [rax],al
	...

Disassembly of section .rela.dyn:

0000000000000418 <.rela.dyn>:
 418:	b8 0d 20 00 00       	mov    eax,0x200d
 41d:	00 00                	add    BYTE PTR [rax],al
 41f:	00 08                	add    BYTE PTR [rax],cl
 421:	00 00                	add    BYTE PTR [rax],al
 423:	00 00                	add    BYTE PTR [rax],al
 425:	00 00                	add    BYTE PTR [rax],al
 427:	00 40 06             	add    BYTE PTR [rax+0x6],al
 42a:	00 00                	add    BYTE PTR [rax],al
 42c:	00 00                	add    BYTE PTR [rax],al
 42e:	00 00                	add    BYTE PTR [rax],al
 430:	c0 0d 20 00 00 00 00 	ror    BYTE PTR [rip+0x20],0x0        # 457 <_init-0x99>
 437:	00 08                	add    BYTE PTR [rax],cl
	...
 441:	06                   	(bad)  
 442:	00 00                	add    BYTE PTR [rax],al
 444:	00 00                	add    BYTE PTR [rax],al
 446:	00 00                	add    BYTE PTR [rax],al
 448:	08 10                	or     BYTE PTR [rax],dl
 44a:	20 00                	and    BYTE PTR [rax],al
 44c:	00 00                	add    BYTE PTR [rax],al
 44e:	00 00                	add    BYTE PTR [rax],al
 450:	08 00                	or     BYTE PTR [rax],al
 452:	00 00                	add    BYTE PTR [rax],al
 454:	00 00                	add    BYTE PTR [rax],al
 456:	00 00                	add    BYTE PTR [rax],al
 458:	08 10                	or     BYTE PTR [rax],dl
 45a:	20 00                	and    BYTE PTR [rax],al
 45c:	00 00                	add    BYTE PTR [rax],al
 45e:	00 00                	add    BYTE PTR [rax],al
 460:	d8 0f                	fmul   DWORD PTR [rdi]
 462:	20 00                	and    BYTE PTR [rax],al
 464:	00 00                	add    BYTE PTR [rax],al
 466:	00 00                	add    BYTE PTR [rax],al
 468:	06                   	(bad)  
 469:	00 00                	add    BYTE PTR [rax],al
 46b:	00 01                	add    BYTE PTR [rcx],al
	...
 475:	00 00                	add    BYTE PTR [rax],al
 477:	00 e0                	add    al,ah
 479:	0f 20 00             	mov    rax,cr0
 47c:	00 00                	add    BYTE PTR [rax],al
 47e:	00 00                	add    BYTE PTR [rax],al
 480:	06                   	(bad)  
 481:	00 00                	add    BYTE PTR [rax],al
 483:	00 03                	add    BYTE PTR [rbx],al
	...
 48d:	00 00                	add    BYTE PTR [rax],al
 48f:	00 e8                	add    al,ch
 491:	0f 20 00             	mov    rax,cr0
 494:	00 00                	add    BYTE PTR [rax],al
 496:	00 00                	add    BYTE PTR [rax],al
 498:	06                   	(bad)  
 499:	00 00                	add    BYTE PTR [rax],al
 49b:	00 04 00             	add    BYTE PTR [rax+rax*1],al
	...
 4a6:	00 00                	add    BYTE PTR [rax],al
 4a8:	f0 0f 20 00          	lock mov rax,cr0
 4ac:	00 00                	add    BYTE PTR [rax],al
 4ae:	00 00                	add    BYTE PTR [rax],al
 4b0:	06                   	(bad)  
 4b1:	00 00                	add    BYTE PTR [rax],al
 4b3:	00 05 00 00 00 00    	add    BYTE PTR [rip+0x0],al        # 4b9 <_init-0x37>
 4b9:	00 00                	add    BYTE PTR [rax],al
 4bb:	00 00                	add    BYTE PTR [rax],al
 4bd:	00 00                	add    BYTE PTR [rax],al
 4bf:	00 f8                	add    al,bh
 4c1:	0f 20 00             	mov    rax,cr0
 4c4:	00 00                	add    BYTE PTR [rax],al
 4c6:	00 00                	add    BYTE PTR [rax],al
 4c8:	06                   	(bad)  
 4c9:	00 00                	add    BYTE PTR [rax],al
 4cb:	00 06                	add    BYTE PTR [rsi],al
	...

Disassembly of section .rela.plt:

00000000000004d8 <.rela.plt>:
 4d8:	d0 0f                	ror    BYTE PTR [rdi],1
 4da:	20 00                	and    BYTE PTR [rax],al
 4dc:	00 00                	add    BYTE PTR [rax],al
 4de:	00 00                	add    BYTE PTR [rax],al
 4e0:	07                   	(bad)  
 4e1:	00 00                	add    BYTE PTR [rax],al
 4e3:	00 02                	add    BYTE PTR [rdx],al
	...

Disassembly of section .init:

00000000000004f0 <_init>:
 4f0:	48 83 ec 08          	sub    rsp,0x8
 4f4:	48 8b 05 ed 0a 20 00 	mov    rax,QWORD PTR [rip+0x200aed]        # 200fe8 <__gmon_start__>
 4fb:	48 85 c0             	test   rax,rax
 4fe:	74 02                	je     502 <_init+0x12>
 500:	ff d0                	call   rax
 502:	48 83 c4 08          	add    rsp,0x8
 506:	c3                   	ret    

Disassembly of section .plt:

0000000000000510 <.plt>:
 510:	ff 35 aa 0a 20 00    	push   QWORD PTR [rip+0x200aaa]        # 200fc0 <_GLOBAL_OFFSET_TABLE_+0x8>
 516:	ff 25 ac 0a 20 00    	jmp    QWORD PTR [rip+0x200aac]        # 200fc8 <_GLOBAL_OFFSET_TABLE_+0x10>
 51c:	0f 1f 40 00          	nop    DWORD PTR [rax+0x0]

0000000000000520 <printf@plt>:
 520:	ff 25 aa 0a 20 00    	jmp    QWORD PTR [rip+0x200aaa]        # 200fd0 <printf@GLIBC_2.2.5>
 526:	68 00 00 00 00       	push   0x0
 52b:	e9 e0 ff ff ff       	jmp    510 <.plt>

Disassembly of section .plt.got:

0000000000000530 <__cxa_finalize@plt>:
 530:	ff 25 c2 0a 20 00    	jmp    QWORD PTR [rip+0x200ac2]        # 200ff8 <__cxa_finalize@GLIBC_2.2.5>
 536:	66 90                	xchg   ax,ax

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
 64a:	55                   	push   rbp
 64b:	48 89 e5             	mov    rbp,rsp
 64e:	89 7d ec             	mov    DWORD PTR [rbp-0x14],edi
 651:	89 75 e8             	mov    DWORD PTR [rbp-0x18],esi
 654:	c7 45 fc 00 00 00 00 	mov    DWORD PTR [rbp-0x4],0x0
 65b:	8b 45 ec             	mov    eax,DWORD PTR [rbp-0x14]
 65e:	01 45 fc             	add    DWORD PTR [rbp-0x4],eax
 661:	8b 45 e8             	mov    eax,DWORD PTR [rbp-0x18]
 664:	01 45 fc             	add    DWORD PTR [rbp-0x4],eax
 667:	8b 45 fc             	mov    eax,DWORD PTR [rbp-0x4]
 66a:	5d                   	pop    rbp
 66b:	c3                   	ret    

000000000000066c <main>:
 66c:	55                   	push   rbp
 66d:	48 89 e5             	mov    rbp,rsp
 670:	48 83 ec 10          	sub    rsp,0x10
 674:	c7 45 f8 02 00 00 00 	mov    DWORD PTR [rbp-0x8],0x2
 67b:	c7 45 fc 03 00 00 00 	mov    DWORD PTR [rbp-0x4],0x3
 682:	8b 55 fc             	mov    edx,DWORD PTR [rbp-0x4]
 685:	8b 45 f8             	mov    eax,DWORD PTR [rbp-0x8]
 688:	89 d6                	mov    esi,edx
 68a:	89 c7                	mov    edi,eax
 68c:	e8 b9 ff ff ff       	call   64a <add>
 691:	89 c6                	mov    esi,eax
 693:	48 8d 3d 9a 00 00 00 	lea    rdi,[rip+0x9a]        # 734 <_IO_stdin_used+0x4>
 69a:	b8 00 00 00 00       	mov    eax,0x0
 69f:	e8 7c fe ff ff       	call   520 <printf@plt>
 6a4:	b8 00 00 00 00       	mov    eax,0x0
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

Disassembly of section .fini:

0000000000000724 <_fini>:
 724:	48 83 ec 08          	sub    rsp,0x8
 728:	48 83 c4 08          	add    rsp,0x8
 72c:	c3                   	ret    

Disassembly of section .rodata:

0000000000000730 <_IO_stdin_used>:
 730:	01 00                	add    DWORD PTR [rax],eax
 732:	02 00                	add    al,BYTE PTR [rax]
 734:	25                   	.byte 0x25
 735:	64 0a 00             	or     al,BYTE PTR fs:[rax]

Disassembly of section .eh_frame_hdr:

0000000000000738 <__GNU_EH_FRAME_HDR>:
 738:	01 1b                	add    DWORD PTR [rbx],ebx
 73a:	03 3b                	add    edi,DWORD PTR [rbx]
 73c:	44 00 00             	add    BYTE PTR [rax],r8b
 73f:	00 07                	add    BYTE PTR [rdi],al
 741:	00 00                	add    BYTE PTR [rax],al
 743:	00 d8                	add    al,bl
 745:	fd                   	std    
 746:	ff                   	(bad)  
 747:	ff 90 00 00 00 f8    	call   QWORD PTR [rax-0x8000000]
 74d:	fd                   	std    
 74e:	ff                   	(bad)  
 74f:	ff                   	(bad)  
 750:	b8 00 00 00 08       	mov    eax,0x8000000
 755:	fe                   	(bad)  
 756:	ff                   	(bad)  
 757:	ff 60 00             	jmp    QWORD PTR [rax+0x0]
 75a:	00 00                	add    BYTE PTR [rax],al
 75c:	12 ff                	adc    bh,bh
 75e:	ff                   	(bad)  
 75f:	ff d0                	call   rax
 761:	00 00                	add    BYTE PTR [rax],al
 763:	00 34 ff             	add    BYTE PTR [rdi+rdi*8],dh
 766:	ff                   	(bad)  
 767:	ff f0                	push   rax
 769:	00 00                	add    BYTE PTR [rax],al
 76b:	00 78 ff             	add    BYTE PTR [rax-0x1],bh
 76e:	ff                   	(bad)  
 76f:	ff 10                	call   QWORD PTR [rax]
 771:	01 00                	add    DWORD PTR [rax],eax
 773:	00 e8                	add    al,ch
 775:	ff                   	(bad)  
 776:	ff                   	(bad)  
 777:	ff 58 01             	call   FWORD PTR [rax+0x1]
	...

Disassembly of section .eh_frame:

0000000000000780 <__FRAME_END__-0x124>:
 780:	14 00                	adc    al,0x0
 782:	00 00                	add    BYTE PTR [rax],al
 784:	00 00                	add    BYTE PTR [rax],al
 786:	00 00                	add    BYTE PTR [rax],al
 788:	01 7a 52             	add    DWORD PTR [rdx+0x52],edi
 78b:	00 01                	add    BYTE PTR [rcx],al
 78d:	78 10                	js     79f <__GNU_EH_FRAME_HDR+0x67>
 78f:	01 1b                	add    DWORD PTR [rbx],ebx
 791:	0c 07                	or     al,0x7
 793:	08 90 01 07 10 14    	or     BYTE PTR [rax+0x14100701],dl
 799:	00 00                	add    BYTE PTR [rax],al
 79b:	00 1c 00             	add    BYTE PTR [rax+rax*1],bl
 79e:	00 00                	add    BYTE PTR [rax],al
 7a0:	a0 fd ff ff 2b 00 00 	movabs al,ds:0x2bfffffd
 7a7:	00 00 
 7a9:	00 00                	add    BYTE PTR [rax],al
 7ab:	00 00                	add    BYTE PTR [rax],al
 7ad:	00 00                	add    BYTE PTR [rax],al
 7af:	00 14 00             	add    BYTE PTR [rax+rax*1],dl
 7b2:	00 00                	add    BYTE PTR [rax],al
 7b4:	00 00                	add    BYTE PTR [rax],al
 7b6:	00 00                	add    BYTE PTR [rax],al
 7b8:	01 7a 52             	add    DWORD PTR [rdx+0x52],edi
 7bb:	00 01                	add    BYTE PTR [rcx],al
 7bd:	78 10                	js     7cf <__GNU_EH_FRAME_HDR+0x97>
 7bf:	01 1b                	add    DWORD PTR [rbx],ebx
 7c1:	0c 07                	or     al,0x7
 7c3:	08 90 01 00 00 24    	or     BYTE PTR [rax+0x24000001],dl
 7c9:	00 00                	add    BYTE PTR [rax],al
 7cb:	00 1c 00             	add    BYTE PTR [rax+rax*1],bl
 7ce:	00 00                	add    BYTE PTR [rax],al
 7d0:	40 fd                	rex std 
 7d2:	ff                   	(bad)  
 7d3:	ff 20                	jmp    QWORD PTR [rax]
 7d5:	00 00                	add    BYTE PTR [rax],al
 7d7:	00 00                	add    BYTE PTR [rax],al
 7d9:	0e                   	(bad)  
 7da:	10 46 0e             	adc    BYTE PTR [rsi+0xe],al
 7dd:	18 4a 0f             	sbb    BYTE PTR [rdx+0xf],cl
 7e0:	0b 77 08             	or     esi,DWORD PTR [rdi+0x8]
 7e3:	80 00 3f             	add    BYTE PTR [rax],0x3f
 7e6:	1a 3b                	sbb    bh,BYTE PTR [rbx]
 7e8:	2a 33                	sub    dh,BYTE PTR [rbx]
 7ea:	24 22                	and    al,0x22
 7ec:	00 00                	add    BYTE PTR [rax],al
 7ee:	00 00                	add    BYTE PTR [rax],al
 7f0:	14 00                	adc    al,0x0
 7f2:	00 00                	add    BYTE PTR [rax],al
 7f4:	44 00 00             	add    BYTE PTR [rax],r8b
 7f7:	00 38                	add    BYTE PTR [rax],bh
 7f9:	fd                   	std    
 7fa:	ff                   	(bad)  
 7fb:	ff 08                	dec    DWORD PTR [rax]
	...
 805:	00 00                	add    BYTE PTR [rax],al
 807:	00 1c 00             	add    BYTE PTR [rax+rax*1],bl
 80a:	00 00                	add    BYTE PTR [rax],al
 80c:	5c                   	pop    rsp
 80d:	00 00                	add    BYTE PTR [rax],al
 80f:	00 3a                	add    BYTE PTR [rdx],bh
 811:	fe                   	(bad)  
 812:	ff                   	(bad)  
 813:	ff 22                	jmp    QWORD PTR [rdx]
 815:	00 00                	add    BYTE PTR [rax],al
 817:	00 00                	add    BYTE PTR [rax],al
 819:	41 0e                	rex.B (bad) 
 81b:	10 86 02 43 0d 06    	adc    BYTE PTR [rsi+0x60d4302],al
 821:	5d                   	pop    rbp
 822:	0c 07                	or     al,0x7
 824:	08 00                	or     BYTE PTR [rax],al
 826:	00 00                	add    BYTE PTR [rax],al
 828:	1c 00                	sbb    al,0x0
 82a:	00 00                	add    BYTE PTR [rax],al
 82c:	7c 00                	jl     82e <__GNU_EH_FRAME_HDR+0xf6>
 82e:	00 00                	add    BYTE PTR [rax],al
 830:	3c fe                	cmp    al,0xfe
 832:	ff                   	(bad)  
 833:	ff                   	(bad)  
 834:	3f                   	(bad)  
 835:	00 00                	add    BYTE PTR [rax],al
 837:	00 00                	add    BYTE PTR [rax],al
 839:	41 0e                	rex.B (bad) 
 83b:	10 86 02 43 0d 06    	adc    BYTE PTR [rsi+0x60d4302],al
 841:	7a 0c                	jp     84f <__GNU_EH_FRAME_HDR+0x117>
 843:	07                   	(bad)  
 844:	08 00                	or     BYTE PTR [rax],al
 846:	00 00                	add    BYTE PTR [rax],al
 848:	44 00 00             	add    BYTE PTR [rax],r8b
 84b:	00 9c 00 00 00 60 fe 	add    BYTE PTR [rax+rax*1-0x1a00000],bl
 852:	ff                   	(bad)  
 853:	ff 65 00             	jmp    QWORD PTR [rbp+0x0]
 856:	00 00                	add    BYTE PTR [rax],al
 858:	00 42 0e             	add    BYTE PTR [rdx+0xe],al
 85b:	10 8f 02 42 0e 18    	adc    BYTE PTR [rdi+0x180e4202],cl
 861:	8e 03                	mov    es,WORD PTR [rbx]
 863:	45 0e                	rex.RB (bad) 
 865:	20 8d 04 42 0e 28    	and    BYTE PTR [rbp+0x280e4204],cl
 86b:	8c 05 48 0e 30 86    	mov    WORD PTR [rip+0xffffffff86300e48],es        # ffffffff863016b9 <_end+0xffffffff861006a1>
 871:	06                   	(bad)  
 872:	48 0e                	rex.W (bad) 
 874:	38 83 07 4d 0e 40    	cmp    BYTE PTR [rbx+0x400e4d07],al
 87a:	72 0e                	jb     88a <__GNU_EH_FRAME_HDR+0x152>
 87c:	38 41 0e             	cmp    BYTE PTR [rcx+0xe],al
 87f:	30 41 0e             	xor    BYTE PTR [rcx+0xe],al
 882:	28 42 0e             	sub    BYTE PTR [rdx+0xe],al
 885:	20 42 0e             	and    BYTE PTR [rdx+0xe],al
 888:	18 42 0e             	sbb    BYTE PTR [rdx+0xe],al
 88b:	10 42 0e             	adc    BYTE PTR [rdx+0xe],al
 88e:	08 00                	or     BYTE PTR [rax],al
 890:	10 00                	adc    BYTE PTR [rax],al
 892:	00 00                	add    BYTE PTR [rax],al
 894:	e4 00                	in     al,0x0
 896:	00 00                	add    BYTE PTR [rax],al
 898:	88 fe                	mov    dh,bh
 89a:	ff                   	(bad)  
 89b:	ff 02                	inc    DWORD PTR [rdx]
 89d:	00 00                	add    BYTE PTR [rax],al
 89f:	00 00                	add    BYTE PTR [rax],al
 8a1:	00 00                	add    BYTE PTR [rax],al
	...

00000000000008a4 <__FRAME_END__>:
 8a4:	00 00                	add    BYTE PTR [rax],al
	...

Disassembly of section .init_array:

0000000000200db8 <__frame_dummy_init_array_entry>:
  200db8:	40 06                	rex (bad) 
  200dba:	00 00                	add    BYTE PTR [rax],al
  200dbc:	00 00                	add    BYTE PTR [rax],al
	...

Disassembly of section .fini_array:

0000000000200dc0 <__do_global_dtors_aux_fini_array_entry>:
  200dc0:	00 06                	add    BYTE PTR [rsi],al
  200dc2:	00 00                	add    BYTE PTR [rax],al
  200dc4:	00 00                	add    BYTE PTR [rax],al
	...

Disassembly of section .dynamic:

0000000000200dc8 <_DYNAMIC>:
  200dc8:	01 00                	add    DWORD PTR [rax],eax
  200dca:	00 00                	add    BYTE PTR [rax],al
  200dcc:	00 00                	add    BYTE PTR [rax],al
  200dce:	00 00                	add    BYTE PTR [rax],al
  200dd0:	01 00                	add    DWORD PTR [rax],eax
  200dd2:	00 00                	add    BYTE PTR [rax],al
  200dd4:	00 00                	add    BYTE PTR [rax],al
  200dd6:	00 00                	add    BYTE PTR [rax],al
  200dd8:	0c 00                	or     al,0x0
  200dda:	00 00                	add    BYTE PTR [rax],al
  200ddc:	00 00                	add    BYTE PTR [rax],al
  200dde:	00 00                	add    BYTE PTR [rax],al
  200de0:	f0 04 00             	lock add al,0x0
  200de3:	00 00                	add    BYTE PTR [rax],al
  200de5:	00 00                	add    BYTE PTR [rax],al
  200de7:	00 0d 00 00 00 00    	add    BYTE PTR [rip+0x0],cl        # 200ded <_DYNAMIC+0x25>
  200ded:	00 00                	add    BYTE PTR [rax],al
  200def:	00 24 07             	add    BYTE PTR [rdi+rax*1],ah
  200df2:	00 00                	add    BYTE PTR [rax],al
  200df4:	00 00                	add    BYTE PTR [rax],al
  200df6:	00 00                	add    BYTE PTR [rax],al
  200df8:	19 00                	sbb    DWORD PTR [rax],eax
  200dfa:	00 00                	add    BYTE PTR [rax],al
  200dfc:	00 00                	add    BYTE PTR [rax],al
  200dfe:	00 00                	add    BYTE PTR [rax],al
  200e00:	b8 0d 20 00 00       	mov    eax,0x200d
  200e05:	00 00                	add    BYTE PTR [rax],al
  200e07:	00 1b                	add    BYTE PTR [rbx],bl
  200e09:	00 00                	add    BYTE PTR [rax],al
  200e0b:	00 00                	add    BYTE PTR [rax],al
  200e0d:	00 00                	add    BYTE PTR [rax],al
  200e0f:	00 08                	add    BYTE PTR [rax],cl
  200e11:	00 00                	add    BYTE PTR [rax],al
  200e13:	00 00                	add    BYTE PTR [rax],al
  200e15:	00 00                	add    BYTE PTR [rax],al
  200e17:	00 1a                	add    BYTE PTR [rdx],bl
  200e19:	00 00                	add    BYTE PTR [rax],al
  200e1b:	00 00                	add    BYTE PTR [rax],al
  200e1d:	00 00                	add    BYTE PTR [rax],al
  200e1f:	00 c0                	add    al,al
  200e21:	0d 20 00 00 00       	or     eax,0x20
  200e26:	00 00                	add    BYTE PTR [rax],al
  200e28:	1c 00                	sbb    al,0x0
  200e2a:	00 00                	add    BYTE PTR [rax],al
  200e2c:	00 00                	add    BYTE PTR [rax],al
  200e2e:	00 00                	add    BYTE PTR [rax],al
  200e30:	08 00                	or     BYTE PTR [rax],al
  200e32:	00 00                	add    BYTE PTR [rax],al
  200e34:	00 00                	add    BYTE PTR [rax],al
  200e36:	00 00                	add    BYTE PTR [rax],al
  200e38:	f5                   	cmc    
  200e39:	fe                   	(bad)  
  200e3a:	ff 6f 00             	jmp    FWORD PTR [rdi+0x0]
  200e3d:	00 00                	add    BYTE PTR [rax],al
  200e3f:	00 98 02 00 00 00    	add    BYTE PTR [rax+0x2],bl
  200e45:	00 00                	add    BYTE PTR [rax],al
  200e47:	00 05 00 00 00 00    	add    BYTE PTR [rip+0x0],al        # 200e4d <_DYNAMIC+0x85>
  200e4d:	00 00                	add    BYTE PTR [rax],al
  200e4f:	00 60 03             	add    BYTE PTR [rax+0x3],ah
  200e52:	00 00                	add    BYTE PTR [rax],al
  200e54:	00 00                	add    BYTE PTR [rax],al
  200e56:	00 00                	add    BYTE PTR [rax],al
  200e58:	06                   	(bad)  
  200e59:	00 00                	add    BYTE PTR [rax],al
  200e5b:	00 00                	add    BYTE PTR [rax],al
  200e5d:	00 00                	add    BYTE PTR [rax],al
  200e5f:	00 b8 02 00 00 00    	add    BYTE PTR [rax+0x2],bh
  200e65:	00 00                	add    BYTE PTR [rax],al
  200e67:	00 0a                	add    BYTE PTR [rdx],cl
  200e69:	00 00                	add    BYTE PTR [rax],al
  200e6b:	00 00                	add    BYTE PTR [rax],al
  200e6d:	00 00                	add    BYTE PTR [rax],al
  200e6f:	00 84 00 00 00 00 00 	add    BYTE PTR [rax+rax*1+0x0],al
  200e76:	00 00                	add    BYTE PTR [rax],al
  200e78:	0b 00                	or     eax,DWORD PTR [rax]
  200e7a:	00 00                	add    BYTE PTR [rax],al
  200e7c:	00 00                	add    BYTE PTR [rax],al
  200e7e:	00 00                	add    BYTE PTR [rax],al
  200e80:	18 00                	sbb    BYTE PTR [rax],al
  200e82:	00 00                	add    BYTE PTR [rax],al
  200e84:	00 00                	add    BYTE PTR [rax],al
  200e86:	00 00                	add    BYTE PTR [rax],al
  200e88:	15 00 00 00 00       	adc    eax,0x0
	...
  200e95:	00 00                	add    BYTE PTR [rax],al
  200e97:	00 03                	add    BYTE PTR [rbx],al
  200e99:	00 00                	add    BYTE PTR [rax],al
  200e9b:	00 00                	add    BYTE PTR [rax],al
  200e9d:	00 00                	add    BYTE PTR [rax],al
  200e9f:	00 b8 0f 20 00 00    	add    BYTE PTR [rax+0x200f],bh
  200ea5:	00 00                	add    BYTE PTR [rax],al
  200ea7:	00 02                	add    BYTE PTR [rdx],al
  200ea9:	00 00                	add    BYTE PTR [rax],al
  200eab:	00 00                	add    BYTE PTR [rax],al
  200ead:	00 00                	add    BYTE PTR [rax],al
  200eaf:	00 18                	add    BYTE PTR [rax],bl
  200eb1:	00 00                	add    BYTE PTR [rax],al
  200eb3:	00 00                	add    BYTE PTR [rax],al
  200eb5:	00 00                	add    BYTE PTR [rax],al
  200eb7:	00 14 00             	add    BYTE PTR [rax+rax*1],dl
  200eba:	00 00                	add    BYTE PTR [rax],al
  200ebc:	00 00                	add    BYTE PTR [rax],al
  200ebe:	00 00                	add    BYTE PTR [rax],al
  200ec0:	07                   	(bad)  
  200ec1:	00 00                	add    BYTE PTR [rax],al
  200ec3:	00 00                	add    BYTE PTR [rax],al
  200ec5:	00 00                	add    BYTE PTR [rax],al
  200ec7:	00 17                	add    BYTE PTR [rdi],dl
  200ec9:	00 00                	add    BYTE PTR [rax],al
  200ecb:	00 00                	add    BYTE PTR [rax],al
  200ecd:	00 00                	add    BYTE PTR [rax],al
  200ecf:	00 d8                	add    al,bl
  200ed1:	04 00                	add    al,0x0
  200ed3:	00 00                	add    BYTE PTR [rax],al
  200ed5:	00 00                	add    BYTE PTR [rax],al
  200ed7:	00 07                	add    BYTE PTR [rdi],al
  200ed9:	00 00                	add    BYTE PTR [rax],al
  200edb:	00 00                	add    BYTE PTR [rax],al
  200edd:	00 00                	add    BYTE PTR [rax],al
  200edf:	00 18                	add    BYTE PTR [rax],bl
  200ee1:	04 00                	add    al,0x0
  200ee3:	00 00                	add    BYTE PTR [rax],al
  200ee5:	00 00                	add    BYTE PTR [rax],al
  200ee7:	00 08                	add    BYTE PTR [rax],cl
  200ee9:	00 00                	add    BYTE PTR [rax],al
  200eeb:	00 00                	add    BYTE PTR [rax],al
  200eed:	00 00                	add    BYTE PTR [rax],al
  200eef:	00 c0                	add    al,al
  200ef1:	00 00                	add    BYTE PTR [rax],al
  200ef3:	00 00                	add    BYTE PTR [rax],al
  200ef5:	00 00                	add    BYTE PTR [rax],al
  200ef7:	00 09                	add    BYTE PTR [rcx],cl
  200ef9:	00 00                	add    BYTE PTR [rax],al
  200efb:	00 00                	add    BYTE PTR [rax],al
  200efd:	00 00                	add    BYTE PTR [rax],al
  200eff:	00 18                	add    BYTE PTR [rax],bl
  200f01:	00 00                	add    BYTE PTR [rax],al
  200f03:	00 00                	add    BYTE PTR [rax],al
  200f05:	00 00                	add    BYTE PTR [rax],al
  200f07:	00 1e                	add    BYTE PTR [rsi],bl
  200f09:	00 00                	add    BYTE PTR [rax],al
  200f0b:	00 00                	add    BYTE PTR [rax],al
  200f0d:	00 00                	add    BYTE PTR [rax],al
  200f0f:	00 08                	add    BYTE PTR [rax],cl
  200f11:	00 00                	add    BYTE PTR [rax],al
  200f13:	00 00                	add    BYTE PTR [rax],al
  200f15:	00 00                	add    BYTE PTR [rax],al
  200f17:	00 fb                	add    bl,bh
  200f19:	ff                   	(bad)  
  200f1a:	ff 6f 00             	jmp    FWORD PTR [rdi+0x0]
  200f1d:	00 00                	add    BYTE PTR [rax],al
  200f1f:	00 01                	add    BYTE PTR [rcx],al
  200f21:	00 00                	add    BYTE PTR [rax],al
  200f23:	08 00                	or     BYTE PTR [rax],al
  200f25:	00 00                	add    BYTE PTR [rax],al
  200f27:	00 fe                	add    dh,bh
  200f29:	ff                   	(bad)  
  200f2a:	ff 6f 00             	jmp    FWORD PTR [rdi+0x0]
  200f2d:	00 00                	add    BYTE PTR [rax],al
  200f2f:	00 f8                	add    al,bh
  200f31:	03 00                	add    eax,DWORD PTR [rax]
  200f33:	00 00                	add    BYTE PTR [rax],al
  200f35:	00 00                	add    BYTE PTR [rax],al
  200f37:	00 ff                	add    bh,bh
  200f39:	ff                   	(bad)  
  200f3a:	ff 6f 00             	jmp    FWORD PTR [rdi+0x0]
  200f3d:	00 00                	add    BYTE PTR [rax],al
  200f3f:	00 01                	add    BYTE PTR [rcx],al
  200f41:	00 00                	add    BYTE PTR [rax],al
  200f43:	00 00                	add    BYTE PTR [rax],al
  200f45:	00 00                	add    BYTE PTR [rax],al
  200f47:	00 f0                	add    al,dh
  200f49:	ff                   	(bad)  
  200f4a:	ff 6f 00             	jmp    FWORD PTR [rdi+0x0]
  200f4d:	00 00                	add    BYTE PTR [rax],al
  200f4f:	00 e4                	add    ah,ah
  200f51:	03 00                	add    eax,DWORD PTR [rax]
  200f53:	00 00                	add    BYTE PTR [rax],al
  200f55:	00 00                	add    BYTE PTR [rax],al
  200f57:	00 f9                	add    cl,bh
  200f59:	ff                   	(bad)  
  200f5a:	ff 6f 00             	jmp    FWORD PTR [rdi+0x0]
  200f5d:	00 00                	add    BYTE PTR [rax],al
  200f5f:	00 03                	add    BYTE PTR [rbx],al
	...

Disassembly of section .got:

0000000000200fb8 <_GLOBAL_OFFSET_TABLE_>:
  200fb8:	c8 0d 20 00          	enter  0x200d,0x0
	...
  200fd0:	26 05 00 00 00 00    	es add eax,0x0
	...

Disassembly of section .data:

0000000000201000 <__data_start>:
	...

0000000000201008 <__dso_handle>:
  201008:	08 10                	or     BYTE PTR [rax],dl
  20100a:	20 00                	and    BYTE PTR [rax],al
  20100c:	00 00                	add    BYTE PTR [rax],al
	...

Disassembly of section .bss:

0000000000201010 <__bss_start>:
	...

Disassembly of section .comment:

0000000000000000 <.comment>:
   0:	47                   	rex.RXB
   1:	43                   	rex.XB
   2:	43 3a 20             	rex.XB cmp spl,BYTE PTR [r8]
   5:	28 55 62             	sub    BYTE PTR [rbp+0x62],dl
   8:	75 6e                	jne    78 <_init-0x478>
   a:	74 75                	je     81 <_init-0x46f>
   c:	20 37                	and    BYTE PTR [rdi],dh
   e:	2e 35 2e 30 2d 33    	cs xor eax,0x332d302e
  14:	75 62                	jne    78 <_init-0x478>
  16:	75 6e                	jne    86 <_init-0x46a>
  18:	74 75                	je     8f <_init-0x461>
  1a:	31 7e 31             	xor    DWORD PTR [rsi+0x31],edi
  1d:	38 2e                	cmp    BYTE PTR [rsi],ch
  1f:	30 34 29             	xor    BYTE PTR [rcx+rbp*1],dh
  22:	20 37                	and    BYTE PTR [rdi],dh
  24:	2e                   	cs
  25:	35                   	.byte 0x35
  26:	2e 30 00             	xor    BYTE PTR cs:[rax],al

Disassembly of section .debug_aranges:

0000000000000000 <.debug_aranges>:
   0:	2c 00                	sub    al,0x0
   2:	00 00                	add    BYTE PTR [rax],al
   4:	02 00                	add    al,BYTE PTR [rax]
   6:	00 00                	add    BYTE PTR [rax],al
   8:	00 00                	add    BYTE PTR [rax],al
   a:	08 00                	or     BYTE PTR [rax],al
   c:	00 00                	add    BYTE PTR [rax],al
   e:	00 00                	add    BYTE PTR [rax],al
  10:	4a 06                	rex.WX (bad) 
  12:	00 00                	add    BYTE PTR [rax],al
  14:	00 00                	add    BYTE PTR [rax],al
  16:	00 00                	add    BYTE PTR [rax],al
  18:	61                   	(bad)  
	...

Disassembly of section .debug_info:

0000000000000000 <.debug_info>:
   0:	7a 03                	jp     5 <_init-0x4eb>
   2:	00 00                	add    BYTE PTR [rax],al
   4:	04 00                	add    al,0x0
   6:	00 00                	add    BYTE PTR [rax],al
   8:	00 00                	add    BYTE PTR [rax],al
   a:	08 01                	or     BYTE PTR [rcx],al
   c:	b7 01                	mov    bh,0x1
   e:	00 00                	add    BYTE PTR [rax],al
  10:	0c ed                	or     al,0xed
  12:	00 00                	add    BYTE PTR [rax],al
  14:	00 61 00             	add    BYTE PTR [rcx+0x0],ah
  17:	00 00                	add    BYTE PTR [rax],al
  19:	4a 06                	rex.WX (bad) 
  1b:	00 00                	add    BYTE PTR [rax],al
  1d:	00 00                	add    BYTE PTR [rax],al
  1f:	00 00                	add    BYTE PTR [rax],al
  21:	61                   	(bad)  
	...
  2a:	00 00                	add    BYTE PTR [rax],al
  2c:	00 02                	add    BYTE PTR [rdx],al
  2e:	38 00                	cmp    BYTE PTR [rax],al
  30:	00 00                	add    BYTE PTR [rax],al
  32:	02 d8                	add    bl,al
  34:	38 00                	cmp    BYTE PTR [rax],al
  36:	00 00                	add    BYTE PTR [rax],al
  38:	03 08                	add    ecx,DWORD PTR [rax]
  3a:	07                   	(bad)  
  3b:	7e 01                	jle    3e <_init-0x4b2>
  3d:	00 00                	add    BYTE PTR [rax],al
  3f:	03 01                	add    eax,DWORD PTR [rcx]
  41:	08 df                	or     bh,bl
  43:	00 00                	add    BYTE PTR [rax],al
  45:	00 03                	add    BYTE PTR [rbx],al
  47:	02 07                	add    al,BYTE PTR [rdi]
  49:	3d 01 00 00 03       	cmp    eax,0x3000001
  4e:	04 07                	add    al,0x7
  50:	83 01 00             	add    DWORD PTR [rcx],0x0
  53:	00 03                	add    BYTE PTR [rbx],al
  55:	01 06                	add    DWORD PTR [rsi],eax
  57:	e1 00                	loope  59 <_init-0x497>
  59:	00 00                	add    BYTE PTR [rax],al
  5b:	03 02                	add    eax,DWORD PTR [rdx]
  5d:	05 2e 00 00 00       	add    eax,0x2e
  62:	04 04                	add    al,0x4
  64:	05 69 6e 74 00       	add    eax,0x746e69
  69:	03 08                	add    ecx,DWORD PTR [rax]
  6b:	05 98 00 00 00       	add    eax,0x98
  70:	02 a8 01 00 00 03    	add    ch,BYTE PTR [rax+0x3000001]
  76:	8c 69 00             	mov    WORD PTR [rcx+0x0],gs
  79:	00 00                	add    BYTE PTR [rax],al
  7b:	02 9e 01 00 00 03    	add    bl,BYTE PTR [rsi+0x3000001]
  81:	8d 69 00             	lea    ebp,[rcx+0x0]
  84:	00 00                	add    BYTE PTR [rax],al
  86:	05 08 06 08 8e       	add    eax,0x8e080608
  8b:	00 00                	add    BYTE PTR [rax],al
  8d:	00 03                	add    BYTE PTR [rbx],al
  8f:	01 06                	add    DWORD PTR [rsi],eax
  91:	e8 00 00 00 07       	call   7000096 <_end+0x6dff07e>
  96:	8e 00                	mov    es,WORD PTR [rax]
  98:	00 00                	add    BYTE PTR [rax],al
  9a:	08 d6                	or     dh,dl
  9c:	00 00                	add    BYTE PTR [rax],al
  9e:	00 d8                	add    al,bl
  a0:	04 f5                	add    al,0xf5
  a2:	1a 02                	sbb    al,BYTE PTR [rdx]
  a4:	00 00                	add    BYTE PTR [rax],al
  a6:	09 4d 00             	or     DWORD PTR [rbp+0x0],ecx
  a9:	00 00                	add    BYTE PTR [rax],al
  ab:	04 f6                	add    al,0xf6
  ad:	62                   	(bad)  
  ae:	00 00                	add    BYTE PTR [rax],al
  b0:	00 00                	add    BYTE PTR [rax],al
  b2:	09 30                	or     DWORD PTR [rax],esi
  b4:	01 00                	add    DWORD PTR [rax],eax
  b6:	00 04 fb             	add    BYTE PTR [rbx+rdi*8],al
  b9:	88 00                	mov    BYTE PTR [rax],al
  bb:	00 00                	add    BYTE PTR [rax],al
  bd:	08 09                	or     BYTE PTR [rcx],cl
  bf:	7e 00                	jle    c1 <_init-0x42f>
  c1:	00 00                	add    BYTE PTR [rax],al
  c3:	04 fc                	add    al,0xfc
  c5:	88 00                	mov    BYTE PTR [rax],al
  c7:	00 00                	add    BYTE PTR [rax],al
  c9:	10 09                	adc    BYTE PTR [rcx],cl
  cb:	22 02                	and    al,BYTE PTR [rdx]
  cd:	00 00                	add    BYTE PTR [rax],al
  cf:	04 fd                	add    al,0xfd
  d1:	88 00                	mov    BYTE PTR [rax],al
  d3:	00 00                	add    BYTE PTR [rax],al
  d5:	18 09                	sbb    BYTE PTR [rcx],cl
  d7:	18 01                	sbb    BYTE PTR [rcx],al
  d9:	00 00                	add    BYTE PTR [rax],al
  db:	04 fe                	add    al,0xfe
  dd:	88 00                	mov    BYTE PTR [rax],al
  df:	00 00                	add    BYTE PTR [rax],al
  e1:	20 09                	and    BYTE PTR [rcx],cl
  e3:	3f                   	(bad)  
  e4:	00 00                	add    BYTE PTR [rax],al
  e6:	00 04 ff             	add    BYTE PTR [rdi+rdi*8],al
  e9:	88 00                	mov    BYTE PTR [rax],al
  eb:	00 00                	add    BYTE PTR [rax],al
  ed:	28 0a                	sub    BYTE PTR [rdx],cl
  ef:	90                   	nop
  f0:	01 00                	add    DWORD PTR [rax],eax
  f2:	00 04 00             	add    BYTE PTR [rax+rax*1],al
  f5:	01 88 00 00 00 30    	add    DWORD PTR [rax+0x30000000],ecx
  fb:	0a 54 00 00          	or     dl,BYTE PTR [rax+rax*1+0x0]
  ff:	00 04 01             	add    BYTE PTR [rcx+rax*1],al
 102:	01 88 00 00 00 38    	add    DWORD PTR [rax+0x38000000],ecx
 108:	0a 00                	or     al,BYTE PTR [rax]
 10a:	00 00                	add    BYTE PTR [rax],al
 10c:	00 04 02             	add    BYTE PTR [rdx+rax*1],al
 10f:	01 88 00 00 00 40    	add    DWORD PTR [rax+0x40000000],ecx
 115:	0a 3f                	or     bh,BYTE PTR [rdi]
 117:	02 00                	add    al,BYTE PTR [rax]
 119:	00 04 04             	add    BYTE PTR [rsp+rax*1],al
 11c:	01 88 00 00 00 48    	add    DWORD PTR [rax+0x48000000],ecx
 122:	0a fe                	or     bh,dh
 124:	01 00                	add    DWORD PTR [rax],eax
 126:	00 04 05 01 88 00 00 	add    BYTE PTR [rax*1+0x8801],al
 12d:	00 50 0a             	add    BYTE PTR [rax+0xa],dl
 130:	21 00                	and    DWORD PTR [rax],eax
 132:	00 00                	add    BYTE PTR [rax],al
 134:	04 06                	add    al,0x6
 136:	01 88 00 00 00 58    	add    DWORD PTR [rax+0x58000000],ecx
 13c:	0a 75 00             	or     dh,BYTE PTR [rbp+0x0]
 13f:	00 00                	add    BYTE PTR [rax],al
 141:	04 08                	add    al,0x8
 143:	01 52 02             	add    DWORD PTR [rdx+0x2],edx
 146:	00 00                	add    BYTE PTR [rax],al
 148:	60                   	(bad)  
 149:	0a b0 01 00 00 04    	or     dh,BYTE PTR [rax+0x4000001]
 14f:	0a 01                	or     al,BYTE PTR [rcx]
 151:	58                   	pop    rax
 152:	02 00                	add    al,BYTE PTR [rax]
 154:	00 68 0a             	add    BYTE PTR [rax+0xa],ch
 157:	59                   	pop    rcx
 158:	02 00                	add    al,BYTE PTR [rax]
 15a:	00 04 0c             	add    BYTE PTR [rsp+rcx*1],al
 15d:	01 62 00             	add    DWORD PTR [rdx+0x0],esp
 160:	00 00                	add    BYTE PTR [rax],al
 162:	70 0a                	jo     16e <_init-0x382>
 164:	14 02                	adc    al,0x2
 166:	00 00                	add    BYTE PTR [rax],al
 168:	04 10                	add    al,0x10
 16a:	01 62 00             	add    DWORD PTR [rdx+0x0],esp
 16d:	00 00                	add    BYTE PTR [rax],al
 16f:	74 0a                	je     17b <_init-0x375>
 171:	0c 00                	or     al,0x0
 173:	00 00                	add    BYTE PTR [rax],al
 175:	04 12                	add    al,0x12
 177:	01 70 00             	add    DWORD PTR [rax+0x0],esi
 17a:	00 00                	add    BYTE PTR [rax],al
 17c:	78 0a                	js     188 <_init-0x368>
 17e:	a1 00 00 00 04 16 01 	movabs eax,ds:0x46011604000000
 185:	46 00 
 187:	00 00                	add    BYTE PTR [rax],al
 189:	80 0a 30             	or     BYTE PTR [rdx],0x30
 18c:	02 00                	add    al,BYTE PTR [rax]
 18e:	00 04 17             	add    BYTE PTR [rdi+rdx*1],al
 191:	01 54 00 00          	add    DWORD PTR [rax+rax*1+0x0],edx
 195:	00 82 0a 0e 01 00    	add    BYTE PTR [rdx+0x10e0a],al
 19b:	00 04 18             	add    BYTE PTR [rax+rbx*1],al
 19e:	01 5e 02             	add    DWORD PTR [rsi+0x2],ebx
 1a1:	00 00                	add    BYTE PTR [rax],al
 1a3:	83 0a 92             	or     DWORD PTR [rdx],0xffffff92
 1a6:	00 00                	add    BYTE PTR [rax],al
 1a8:	00 04 1c             	add    BYTE PTR [rsp+rbx*1],al
 1ab:	01 6e 02             	add    DWORD PTR [rsi+0x2],ebp
 1ae:	00 00                	add    BYTE PTR [rax],al
 1b0:	88 0a                	mov    BYTE PTR [rdx],cl
 1b2:	10 00                	adc    BYTE PTR [rax],al
 1b4:	00 00                	add    BYTE PTR [rax],al
 1b6:	04 25                	add    al,0x25
 1b8:	01 7b 00             	add    DWORD PTR [rbx+0x0],edi
 1bb:	00 00                	add    BYTE PTR [rax],al
 1bd:	90                   	nop
 1be:	0a 5b 01             	or     bl,BYTE PTR [rbx+0x1]
 1c1:	00 00                	add    BYTE PTR [rax],al
 1c3:	04 2d                	add    al,0x2d
 1c5:	01 86 00 00 00 98    	add    DWORD PTR [rsi-0x68000000],eax
 1cb:	0a 62 01             	or     ah,BYTE PTR [rdx+0x1]
 1ce:	00 00                	add    BYTE PTR [rax],al
 1d0:	04 2e                	add    al,0x2e
 1d2:	01 86 00 00 00 a0    	add    DWORD PTR [rsi-0x60000000],eax
 1d8:	0a 69 01             	or     ch,BYTE PTR [rcx+0x1]
 1db:	00 00                	add    BYTE PTR [rax],al
 1dd:	04 2f                	add    al,0x2f
 1df:	01 86 00 00 00 a8    	add    DWORD PTR [rsi-0x58000000],eax
 1e5:	0a 70 01             	or     dh,BYTE PTR [rax+0x1]
 1e8:	00 00                	add    BYTE PTR [rax],al
 1ea:	04 30                	add    al,0x30
 1ec:	01 86 00 00 00 b0    	add    DWORD PTR [rsi-0x50000000],eax
 1f2:	0a 77 01             	or     dh,BYTE PTR [rdi+0x1]
 1f5:	00 00                	add    BYTE PTR [rax],al
 1f7:	04 32                	add    al,0x32
 1f9:	01 2d 00 00 00 b8    	add    DWORD PTR [rip+0xffffffffb8000000],ebp        # ffffffffb80001ff <_end+0xffffffffb7dff1e7>
 1ff:	0a 1c 02             	or     bl,BYTE PTR [rdx+rax*1]
 202:	00 00                	add    BYTE PTR [rax],al
 204:	04 33                	add    al,0x33
 206:	01 62 00             	add    DWORD PTR [rdx+0x0],esp
 209:	00 00                	add    BYTE PTR [rax],al
 20b:	c0 0a 27             	ror    BYTE PTR [rdx],0x27
 20e:	01 00                	add    DWORD PTR [rax],eax
 210:	00 04 35 01 74 02 00 	add    BYTE PTR [rsi*1+0x27401],al
 217:	00 c4                	add    ah,al
 219:	00 0b                	add    BYTE PTR [rbx],cl
 21b:	78 02                	js     21f <_init-0x2d1>
 21d:	00 00                	add    BYTE PTR [rax],al
 21f:	04 9a                	add    al,0x9a
 221:	08 03                	or     BYTE PTR [rbx],al
 223:	01 00                	add    DWORD PTR [rax],eax
 225:	00 18                	add    BYTE PTR [rax],bl
 227:	04 a0                	add    al,0xa0
 229:	52                   	push   rdx
 22a:	02 00                	add    al,BYTE PTR [rax]
 22c:	00 09                	add    BYTE PTR [rcx],cl
 22e:	55                   	push   rbp
 22f:	01 00                	add    DWORD PTR [rax],eax
 231:	00 04 a1             	add    BYTE PTR [rcx+riz*4],al
 234:	52                   	push   rdx
 235:	02 00                	add    al,BYTE PTR [rax]
 237:	00 00                	add    BYTE PTR [rax],al
 239:	09 d0                	or     eax,edx
 23b:	00 00                	add    BYTE PTR [rax],al
 23d:	00 04 a2             	add    BYTE PTR [rdx+riz*4],al
 240:	58                   	pop    rax
 241:	02 00                	add    al,BYTE PTR [rax]
 243:	00 08                	add    BYTE PTR [rax],cl
 245:	09 cb                	or     ebx,ecx
 247:	00 00                	add    BYTE PTR [rax],al
 249:	00 04 a6             	add    BYTE PTR [rsi+riz*4],al
 24c:	62                   	(bad)  
 24d:	00 00                	add    BYTE PTR [rax],al
 24f:	00 10                	add    BYTE PTR [rax],dl
 251:	00 06                	add    BYTE PTR [rsi],al
 253:	08 21                	or     BYTE PTR [rcx],ah
 255:	02 00                	add    al,BYTE PTR [rax]
 257:	00 06                	add    BYTE PTR [rsi],al
 259:	08 9a 00 00 00 0c    	or     BYTE PTR [rdx+0xc000000],bl
 25f:	8e 00                	mov    es,WORD PTR [rax]
 261:	00 00                	add    BYTE PTR [rax],al
 263:	6e                   	outs   dx,BYTE PTR ds:[rsi]
 264:	02 00                	add    al,BYTE PTR [rax]
 266:	00 0d 38 00 00 00    	add    BYTE PTR [rip+0x38],cl        # 2a4 <_init-0x24c>
 26c:	00 00                	add    BYTE PTR [rax],al
 26e:	06                   	(bad)  
 26f:	08 1a                	or     BYTE PTR [rdx],bl
 271:	02 00                	add    al,BYTE PTR [rax]
 273:	00 0c 8e             	add    BYTE PTR [rsi+rcx*4],cl
 276:	00 00                	add    BYTE PTR [rax],al
 278:	00 84 02 00 00 0d 38 	add    BYTE PTR [rdx+rax*1+0x380d0000],al
 27f:	00 00                	add    BYTE PTR [rax],al
 281:	00 13                	add    BYTE PTR [rbx],dl
 283:	00 0e                	add    BYTE PTR [rsi],cl
 285:	bd 00 00 00 0f       	mov    ebp,0xf000000
 28a:	f4                   	hlt    
 28b:	00 00                	add    BYTE PTR [rax],al
 28d:	00 04 3f             	add    BYTE PTR [rdi+rdi*1],al
 290:	01 84 02 00 00 0f 68 	add    DWORD PTR [rdx+rax*1+0x680f0000],eax
 297:	02 00                	add    al,BYTE PTR [rax]
 299:	00 04 40             	add    BYTE PTR [rax+rax*2],al
 29c:	01 84 02 00 00 0f ad 	add    DWORD PTR [rdx+rax*1-0x52f10000],eax
 2a3:	00 00                	add    BYTE PTR [rax],al
 2a5:	00 04 41             	add    BYTE PTR [rcx+rax*2],al
 2a8:	01 84 02 00 00 06 08 	add    DWORD PTR [rdx+rax*1+0x8060000],eax
 2af:	95                   	xchg   ebp,eax
 2b0:	00 00                	add    BYTE PTR [rax],al
 2b2:	00 07                	add    BYTE PTR [rdi],al
 2b4:	ad                   	lods   eax,DWORD PTR ds:[rsi]
 2b5:	02 00                	add    al,BYTE PTR [rax]
 2b7:	00 10                	add    BYTE PTR [rax],dl
 2b9:	0e                   	(bad)  
 2ba:	02 00                	add    al,BYTE PTR [rax]
 2bc:	00 05 87 58 02 00    	add    BYTE PTR [rip+0x25887],al        # 25b49 <__FRAME_END__+0x252a5>
 2c2:	00 10                	add    BYTE PTR [rax],dl
 2c4:	61                   	(bad)  
 2c5:	02 00                	add    al,BYTE PTR [rax]
 2c7:	00 05 88 58 02 00    	add    BYTE PTR [rip+0x25888],al        # 25b55 <__FRAME_END__+0x252b1>
 2cd:	00 10                	add    BYTE PTR [rax],dl
 2cf:	8b 00                	mov    eax,DWORD PTR [rax]
 2d1:	00 00                	add    BYTE PTR [rax],al
 2d3:	05 89 58 02 00       	add    eax,0x25889
 2d8:	00 10                	add    BYTE PTR [rax],dl
 2da:	18 00                	sbb    BYTE PTR [rax],al
 2dc:	00 00                	add    BYTE PTR [rax],al
 2de:	06                   	(bad)  
 2df:	1a 62 00             	sbb    ah,BYTE PTR [rdx+0x0]
 2e2:	00 00                	add    BYTE PTR [rax],al
 2e4:	0c b3                	or     al,0xb3
 2e6:	02 00                	add    al,BYTE PTR [rax]
 2e8:	00 ef                	add    bh,ch
 2ea:	02 00                	add    al,BYTE PTR [rax]
 2ec:	00 11                	add    BYTE PTR [rcx],dl
 2ee:	00 07                	add    BYTE PTR [rdi],al
 2f0:	e4 02                	in     al,0x2
 2f2:	00 00                	add    BYTE PTR [rax],al
 2f4:	10 4d 02             	adc    BYTE PTR [rbp+0x2],cl
 2f7:	00 00                	add    BYTE PTR [rax],al
 2f9:	06                   	(bad)  
 2fa:	1b ef                	sbb    ebp,edi
 2fc:	02 00                	add    al,BYTE PTR [rax]
 2fe:	00 12                	add    BYTE PTR [rdx],dl
 300:	50                   	push   rax
 301:	01 00                	add    DWORD PTR [rax],eax
 303:	00 01                	add    BYTE PTR [rcx],al
 305:	0b 62 00             	or     esp,DWORD PTR [rdx+0x0]
 308:	00 00                	add    BYTE PTR [rax],al
 30a:	6c                   	ins    BYTE PTR es:[rdi],dx
 30b:	06                   	(bad)  
 30c:	00 00                	add    BYTE PTR [rax],al
 30e:	00 00                	add    BYTE PTR [rax],al
 310:	00 00                	add    BYTE PTR [rax],al
 312:	3f                   	(bad)  
 313:	00 00                	add    BYTE PTR [rax],al
 315:	00 00                	add    BYTE PTR [rax],al
 317:	00 00                	add    BYTE PTR [rax],al
 319:	00 01                	add    BYTE PTR [rcx],al
 31b:	9c                   	pushf  
 31c:	39 03                	cmp    DWORD PTR [rbx],eax
 31e:	00 00                	add    BYTE PTR [rax],al
 320:	13 61 00             	adc    esp,DWORD PTR [rcx+0x0]
 323:	01 0d 62 00 00 00    	add    DWORD PTR [rip+0x62],ecx        # 38b <_init-0x165>
 329:	02 91 68 13 62 00    	add    dl,BYTE PTR [rcx+0x621368]
 32f:	01 0d 62 00 00 00    	add    DWORD PTR [rip+0x62],ecx        # 397 <_init-0x159>
 335:	02 91 6c 00 14 61    	add    dl,BYTE PTR [rcx+0x6114006c]
 33b:	64 64 00 01          	fs add BYTE PTR fs:[rcx],al
 33f:	03 62 00             	add    esp,DWORD PTR [rdx+0x0]
 342:	00 00                	add    BYTE PTR [rax],al
 344:	4a 06                	rex.WX (bad) 
 346:	00 00                	add    BYTE PTR [rax],al
 348:	00 00                	add    BYTE PTR [rax],al
 34a:	00 00                	add    BYTE PTR [rax],al
 34c:	22 00                	and    al,BYTE PTR [rax]
 34e:	00 00                	add    BYTE PTR [rax],al
 350:	00 00                	add    BYTE PTR [rax],al
 352:	00 00                	add    BYTE PTR [rax],al
 354:	01 9c 15 78 00 01 03 	add    DWORD PTR [rbp+rdx*1+0x3010078],ebx
 35b:	62                   	(bad)  
 35c:	00 00                	add    BYTE PTR [rax],al
 35e:	00 02                	add    BYTE PTR [rdx],al
 360:	91                   	xchg   ecx,eax
 361:	5c                   	pop    rsp
 362:	15 79 00 01 03       	adc    eax,0x3010079
 367:	62                   	(bad)  
 368:	00 00                	add    BYTE PTR [rax],al
 36a:	00 02                	add    BYTE PTR [rdx],al
 36c:	91                   	xchg   ecx,eax
 36d:	58                   	pop    rax
 36e:	13 73 75             	adc    esi,DWORD PTR [rbx+0x75]
 371:	6d                   	ins    DWORD PTR es:[rdi],dx
 372:	00 01                	add    BYTE PTR [rcx],al
 374:	05 62 00 00 00       	add    eax,0x62
 379:	02                   	.byte 0x2
 37a:	91                   	xchg   ecx,eax
 37b:	6c                   	ins    BYTE PTR es:[rdi],dx
	...

Disassembly of section .debug_abbrev:

0000000000000000 <.debug_abbrev>:
   0:	01 11                	add    DWORD PTR [rcx],edx
   2:	01 25 0e 13 0b 03    	add    DWORD PTR [rip+0x30b130e],esp        # 30b1316 <_end+0x2eb02fe>
   8:	0e                   	(bad)  
   9:	1b 0e                	sbb    ecx,DWORD PTR [rsi]
   b:	11 01                	adc    DWORD PTR [rcx],eax
   d:	12 07                	adc    al,BYTE PTR [rdi]
   f:	10 17                	adc    BYTE PTR [rdi],dl
  11:	00 00                	add    BYTE PTR [rax],al
  13:	02 16                	add    dl,BYTE PTR [rsi]
  15:	00 03                	add    BYTE PTR [rbx],al
  17:	0e                   	(bad)  
  18:	3a 0b                	cmp    cl,BYTE PTR [rbx]
  1a:	3b 0b                	cmp    ecx,DWORD PTR [rbx]
  1c:	49 13 00             	adc    rax,QWORD PTR [r8]
  1f:	00 03                	add    BYTE PTR [rbx],al
  21:	24 00                	and    al,0x0
  23:	0b 0b                	or     ecx,DWORD PTR [rbx]
  25:	3e 0b 03             	or     eax,DWORD PTR ds:[rbx]
  28:	0e                   	(bad)  
  29:	00 00                	add    BYTE PTR [rax],al
  2b:	04 24                	add    al,0x24
  2d:	00 0b                	add    BYTE PTR [rbx],cl
  2f:	0b 3e                	or     edi,DWORD PTR [rsi]
  31:	0b 03                	or     eax,DWORD PTR [rbx]
  33:	08 00                	or     BYTE PTR [rax],al
  35:	00 05 0f 00 0b 0b    	add    BYTE PTR [rip+0xb0b000f],al        # b0b004a <_end+0xaeaf032>
  3b:	00 00                	add    BYTE PTR [rax],al
  3d:	06                   	(bad)  
  3e:	0f 00 0b             	str    WORD PTR [rbx]
  41:	0b 49 13             	or     ecx,DWORD PTR [rcx+0x13]
  44:	00 00                	add    BYTE PTR [rax],al
  46:	07                   	(bad)  
  47:	26 00 49 13          	add    BYTE PTR es:[rcx+0x13],cl
  4b:	00 00                	add    BYTE PTR [rax],al
  4d:	08 13                	or     BYTE PTR [rbx],dl
  4f:	01 03                	add    DWORD PTR [rbx],eax
  51:	0e                   	(bad)  
  52:	0b 0b                	or     ecx,DWORD PTR [rbx]
  54:	3a 0b                	cmp    cl,BYTE PTR [rbx]
  56:	3b 0b                	cmp    ecx,DWORD PTR [rbx]
  58:	01 13                	add    DWORD PTR [rbx],edx
  5a:	00 00                	add    BYTE PTR [rax],al
  5c:	09 0d 00 03 0e 3a    	or     DWORD PTR [rip+0x3a0e0300],ecx        # 3a0e0362 <_end+0x39edf34a>
  62:	0b 3b                	or     edi,DWORD PTR [rbx]
  64:	0b 49 13             	or     ecx,DWORD PTR [rcx+0x13]
  67:	38 0b                	cmp    BYTE PTR [rbx],cl
  69:	00 00                	add    BYTE PTR [rax],al
  6b:	0a 0d 00 03 0e 3a    	or     cl,BYTE PTR [rip+0x3a0e0300]        # 3a0e0371 <_end+0x39edf359>
  71:	0b 3b                	or     edi,DWORD PTR [rbx]
  73:	05 49 13 38 0b       	add    eax,0xb381349
  78:	00 00                	add    BYTE PTR [rax],al
  7a:	0b 16                	or     edx,DWORD PTR [rsi]
  7c:	00 03                	add    BYTE PTR [rbx],al
  7e:	0e                   	(bad)  
  7f:	3a 0b                	cmp    cl,BYTE PTR [rbx]
  81:	3b 0b                	cmp    ecx,DWORD PTR [rbx]
  83:	00 00                	add    BYTE PTR [rax],al
  85:	0c 01                	or     al,0x1
  87:	01 49 13             	add    DWORD PTR [rcx+0x13],ecx
  8a:	01 13                	add    DWORD PTR [rbx],edx
  8c:	00 00                	add    BYTE PTR [rax],al
  8e:	0d 21 00 49 13       	or     eax,0x13490021
  93:	2f                   	(bad)  
  94:	0b 00                	or     eax,DWORD PTR [rax]
  96:	00 0e                	add    BYTE PTR [rsi],cl
  98:	13 00                	adc    eax,DWORD PTR [rax]
  9a:	03 0e                	add    ecx,DWORD PTR [rsi]
  9c:	3c 19                	cmp    al,0x19
  9e:	00 00                	add    BYTE PTR [rax],al
  a0:	0f 34                	sysenter 
  a2:	00 03                	add    BYTE PTR [rbx],al
  a4:	0e                   	(bad)  
  a5:	3a 0b                	cmp    cl,BYTE PTR [rbx]
  a7:	3b 05 49 13 3f 19    	cmp    eax,DWORD PTR [rip+0x193f1349]        # 193f13f6 <_end+0x191f03de>
  ad:	3c 19                	cmp    al,0x19
  af:	00 00                	add    BYTE PTR [rax],al
  b1:	10 34 00             	adc    BYTE PTR [rax+rax*1],dh
  b4:	03 0e                	add    ecx,DWORD PTR [rsi]
  b6:	3a 0b                	cmp    cl,BYTE PTR [rbx]
  b8:	3b 0b                	cmp    ecx,DWORD PTR [rbx]
  ba:	49 13 3f             	adc    rdi,QWORD PTR [r15]
  bd:	19 3c 19             	sbb    DWORD PTR [rcx+rbx*1],edi
  c0:	00 00                	add    BYTE PTR [rax],al
  c2:	11 21                	adc    DWORD PTR [rcx],esp
  c4:	00 00                	add    BYTE PTR [rax],al
  c6:	00 12                	add    BYTE PTR [rdx],dl
  c8:	2e 01 3f             	add    DWORD PTR cs:[rdi],edi
  cb:	19 03                	sbb    DWORD PTR [rbx],eax
  cd:	0e                   	(bad)  
  ce:	3a 0b                	cmp    cl,BYTE PTR [rbx]
  d0:	3b 0b                	cmp    ecx,DWORD PTR [rbx]
  d2:	49 13 11             	adc    rdx,QWORD PTR [r9]
  d5:	01 12                	add    DWORD PTR [rdx],edx
  d7:	07                   	(bad)  
  d8:	40 18 96 42 19 01 13 	sbb    BYTE PTR [rsi+0x13011942],dl
  df:	00 00                	add    BYTE PTR [rax],al
  e1:	13 34 00             	adc    esi,DWORD PTR [rax+rax*1]
  e4:	03 08                	add    ecx,DWORD PTR [rax]
  e6:	3a 0b                	cmp    cl,BYTE PTR [rbx]
  e8:	3b 0b                	cmp    ecx,DWORD PTR [rbx]
  ea:	49 13 02             	adc    rax,QWORD PTR [r10]
  ed:	18 00                	sbb    BYTE PTR [rax],al
  ef:	00 14 2e             	add    BYTE PTR [rsi+rbp*1],dl
  f2:	01 3f                	add    DWORD PTR [rdi],edi
  f4:	19 03                	sbb    DWORD PTR [rbx],eax
  f6:	08 3a                	or     BYTE PTR [rdx],bh
  f8:	0b 3b                	or     edi,DWORD PTR [rbx]
  fa:	0b 27                	or     esp,DWORD PTR [rdi]
  fc:	19 49 13             	sbb    DWORD PTR [rcx+0x13],ecx
  ff:	11 01                	adc    DWORD PTR [rcx],eax
 101:	12 07                	adc    al,BYTE PTR [rdi]
 103:	40 18 97 42 19 00 00 	sbb    BYTE PTR [rdi+0x1942],dl
 10a:	15 05 00 03 08       	adc    eax,0x8030005
 10f:	3a 0b                	cmp    cl,BYTE PTR [rbx]
 111:	3b 0b                	cmp    ecx,DWORD PTR [rbx]
 113:	49 13 02             	adc    rax,QWORD PTR [r10]
 116:	18 00                	sbb    BYTE PTR [rax],al
	...

Disassembly of section .debug_line:

0000000000000000 <.debug_line>:
   0:	d6                   	(bad)  
   1:	00 00                	add    BYTE PTR [rax],al
   3:	00 02                	add    BYTE PTR [rdx],al
   5:	00 b3 00 00 00 01    	add    BYTE PTR [rbx+0x1000000],dh
   b:	01 fb                	add    ebx,edi
   d:	0e                   	(bad)  
   e:	0d 00 01 01 01       	or     eax,0x1010100
  13:	01 00                	add    DWORD PTR [rax],eax
  15:	00 00                	add    BYTE PTR [rax],al
  17:	01 00                	add    DWORD PTR [rax],eax
  19:	00 01                	add    BYTE PTR [rcx],al
  1b:	2f                   	(bad)  
  1c:	75 73                	jne    91 <_init-0x45f>
  1e:	72 2f                	jb     4f <_init-0x4a1>
  20:	6c                   	ins    BYTE PTR es:[rdi],dx
  21:	69 62 2f 67 63 63 2f 	imul   esp,DWORD PTR [rdx+0x2f],0x2f636367
  28:	78 38                	js     62 <_init-0x48e>
  2a:	36 5f                	ss pop rdi
  2c:	36 34 2d             	ss xor al,0x2d
  2f:	6c                   	ins    BYTE PTR es:[rdi],dx
  30:	69 6e 75 78 2d 67 6e 	imul   ebp,DWORD PTR [rsi+0x75],0x6e672d78
  37:	75 2f                	jne    68 <_init-0x488>
  39:	37                   	(bad)  
  3a:	2f                   	(bad)  
  3b:	69 6e 63 6c 75 64 65 	imul   ebp,DWORD PTR [rsi+0x63],0x6564756c
  42:	00 2f                	add    BYTE PTR [rdi],ch
  44:	75 73                	jne    b9 <_init-0x437>
  46:	72 2f                	jb     77 <_init-0x479>
  48:	69 6e 63 6c 75 64 65 	imul   ebp,DWORD PTR [rsi+0x63],0x6564756c
  4f:	2f                   	(bad)  
  50:	78 38                	js     8a <_init-0x466>
  52:	36 5f                	ss pop rdi
  54:	36 34 2d             	ss xor al,0x2d
  57:	6c                   	ins    BYTE PTR es:[rdi],dx
  58:	69 6e 75 78 2d 67 6e 	imul   ebp,DWORD PTR [rsi+0x75],0x6e672d78
  5f:	75 2f                	jne    90 <_init-0x460>
  61:	62                   	(bad)  
  62:	69 74 73 00 2f 75 73 	imul   esi,DWORD PTR [rbx+rsi*2+0x0],0x7273752f
  69:	72 
  6a:	2f                   	(bad)  
  6b:	69 6e 63 6c 75 64 65 	imul   ebp,DWORD PTR [rsi+0x63],0x6564756c
  72:	00 00                	add    BYTE PTR [rax],al
  74:	61                   	(bad)  
  75:	64 64 32 2e          	fs xor ch,BYTE PTR fs:[rsi]
  79:	63 00                	movsxd eax,DWORD PTR [rax]
  7b:	00 00                	add    BYTE PTR [rax],al
  7d:	00 73 74             	add    BYTE PTR [rbx+0x74],dh
  80:	64 64 65 66 2e 68 00 	fs fs gs cs pushw 0x100
  87:	01 
  88:	00 00                	add    BYTE PTR [rax],al
  8a:	74 79                	je     105 <_init-0x3eb>
  8c:	70 65                	jo     f3 <_init-0x3fd>
  8e:	73 2e                	jae    be <_init-0x432>
  90:	68 00 02 00 00       	push   0x200
  95:	6c                   	ins    BYTE PTR es:[rdi],dx
  96:	69 62 69 6f 2e 68 00 	imul   esp,DWORD PTR [rdx+0x69],0x682e6f
  9d:	02 00                	add    al,BYTE PTR [rax]
  9f:	00 73 74             	add    BYTE PTR [rbx+0x74],dh
  a2:	64 69 6f 2e 68 00 03 	imul   ebp,DWORD PTR fs:[rdi+0x2e],0x30068
  a9:	00 
  aa:	00 73 79             	add    BYTE PTR [rbx+0x79],dh
  ad:	73 5f                	jae    10e <_init-0x3e2>
  af:	65 72 72             	gs jb  124 <_init-0x3cc>
  b2:	6c                   	ins    BYTE PTR es:[rdi],dx
  b3:	69 73 74 2e 68 00 02 	imul   esi,DWORD PTR [rbx+0x74],0x200682e
  ba:	00 00                	add    BYTE PTR [rax],al
  bc:	00 00                	add    BYTE PTR [rax],al
  be:	09 02                	or     DWORD PTR [rdx],eax
  c0:	4a 06                	rex.WX (bad) 
  c2:	00 00                	add    BYTE PTR [rax],al
  c4:	00 00                	add    BYTE PTR [rax],al
  c6:	00 00                	add    BYTE PTR [rax],al
  c8:	15 9f 75 67 67       	adc    eax,0x6767759f
  cd:	3d 31 83 d7 02       	cmp    eax,0x2d78331
  d2:	22 13                	and    dl,BYTE PTR [rbx]
  d4:	59                   	pop    rcx
  d5:	02 02                	add    al,BYTE PTR [rdx]
  d7:	00 01                	add    BYTE PTR [rcx],al
  d9:	01                   	.byte 0x1

Disassembly of section .debug_str:

0000000000000000 <.debug_str>:
   0:	5f                   	pop    rdi
   1:	49                   	rex.WB
   2:	4f 5f                	rex.WRXB pop r15
   4:	62                   	(bad)  
   5:	75 66                	jne    6d <_init-0x483>
   7:	5f                   	pop    rdi
   8:	65 6e                	outs   dx,BYTE PTR gs:[rsi]
   a:	64 00 5f 6f          	add    BYTE PTR fs:[rdi+0x6f],bl
   e:	6c                   	ins    BYTE PTR es:[rdi],dx
   f:	64 5f                	fs pop rdi
  11:	6f                   	outs   dx,DWORD PTR ds:[rsi]
  12:	66 66 73 65          	data16 data16 jae 7b <_init-0x475>
  16:	74 00                	je     18 <_init-0x4d8>
  18:	73 79                	jae    93 <_init-0x45d>
  1a:	73 5f                	jae    7b <_init-0x475>
  1c:	6e                   	outs   dx,BYTE PTR ds:[rsi]
  1d:	65 72 72             	gs jb  92 <_init-0x45e>
  20:	00 5f 49             	add    BYTE PTR [rdi+0x49],bl
  23:	4f 5f                	rex.WRXB pop r15
  25:	73 61                	jae    88 <_init-0x468>
  27:	76 65                	jbe    8e <_init-0x462>
  29:	5f                   	pop    rdi
  2a:	65 6e                	outs   dx,BYTE PTR gs:[rsi]
  2c:	64 00 73 68          	add    BYTE PTR fs:[rbx+0x68],dh
  30:	6f                   	outs   dx,DWORD PTR ds:[rsi]
  31:	72 74                	jb     a7 <_init-0x449>
  33:	20 69 6e             	and    BYTE PTR [rcx+0x6e],ch
  36:	74 00                	je     38 <_init-0x4b8>
  38:	73 69                	jae    a3 <_init-0x44d>
  3a:	7a 65                	jp     a1 <_init-0x44f>
  3c:	5f                   	pop    rdi
  3d:	74 00                	je     3f <_init-0x4b1>
  3f:	5f                   	pop    rdi
  40:	49                   	rex.WB
  41:	4f 5f                	rex.WRXB pop r15
  43:	77 72                	ja     b7 <_init-0x439>
  45:	69 74 65 5f 70 74 72 	imul   esi,DWORD PTR [rbp+riz*2+0x5f],0x727470
  4c:	00 
  4d:	5f                   	pop    rdi
  4e:	66 6c                	data16 ins BYTE PTR es:[rdi],dx
  50:	61                   	(bad)  
  51:	67 73 00             	addr32 jae 54 <_init-0x49c>
  54:	5f                   	pop    rdi
  55:	49                   	rex.WB
  56:	4f 5f                	rex.WRXB pop r15
  58:	62                   	(bad)  
  59:	75 66                	jne    c1 <_init-0x42f>
  5b:	5f                   	pop    rdi
  5c:	62 61                	(bad)  
  5e:	73 65                	jae    c5 <_init-0x42b>
  60:	00 2f                	add    BYTE PTR [rdi],ch
  62:	68 6f 6d 65 2f       	push   0x2f656d6f
  67:	75 73                	jne    dc <_init-0x414>
  69:	65 72 2f             	gs jb  9b <_init-0x455>
  6c:	32 30                	xor    dh,BYTE PTR [rax]
  6e:	32 34 30             	xor    dh,BYTE PTR [rax+rsi*1]
  71:	31 32                	xor    DWORD PTR [rdx],esi
  73:	37                   	(bad)  
  74:	00 5f 6d             	add    BYTE PTR [rdi+0x6d],bl
  77:	61                   	(bad)  
  78:	72 6b                	jb     e5 <_init-0x40b>
  7a:	65 72 73             	gs jb  f0 <_init-0x400>
  7d:	00 5f 49             	add    BYTE PTR [rdi+0x49],bl
  80:	4f 5f                	rex.WRXB pop r15
  82:	72 65                	jb     e9 <_init-0x407>
  84:	61                   	(bad)  
  85:	64 5f                	fs pop rdi
  87:	65 6e                	outs   dx,BYTE PTR gs:[rsi]
  89:	64 00 73 74          	add    BYTE PTR fs:[rbx+0x74],dh
  8d:	64 65 72 72          	fs gs jb 103 <_init-0x3ed>
  91:	00 5f 6c             	add    BYTE PTR [rdi+0x6c],bl
  94:	6f                   	outs   dx,DWORD PTR ds:[rsi]
  95:	63 6b 00             	movsxd ebp,DWORD PTR [rbx+0x0]
  98:	6c                   	ins    BYTE PTR es:[rdi],dx
  99:	6f                   	outs   dx,DWORD PTR ds:[rsi]
  9a:	6e                   	outs   dx,BYTE PTR ds:[rsi]
  9b:	67 20 69 6e          	and    BYTE PTR [ecx+0x6e],ch
  9f:	74 00                	je     a1 <_init-0x44f>
  a1:	5f                   	pop    rdi
  a2:	63 75 72             	movsxd esi,DWORD PTR [rbp+0x72]
  a5:	5f                   	pop    rdi
  a6:	63 6f 6c             	movsxd ebp,DWORD PTR [rdi+0x6c]
  a9:	75 6d                	jne    118 <_init-0x3d8>
  ab:	6e                   	outs   dx,BYTE PTR ds:[rsi]
  ac:	00 5f 49             	add    BYTE PTR [rdi+0x49],bl
  af:	4f 5f                	rex.WRXB pop r15
  b1:	32 5f 31             	xor    bl,BYTE PTR [rdi+0x31]
  b4:	5f                   	pop    rdi
  b5:	73 74                	jae    12b <_init-0x3c5>
  b7:	64 65 72 72          	fs gs jb 12d <_init-0x3c3>
  bb:	5f                   	pop    rdi
  bc:	00 5f 49             	add    BYTE PTR [rdi+0x49],bl
  bf:	4f 5f                	rex.WRXB pop r15
  c1:	46                   	rex.RX
  c2:	49                   	rex.WB
  c3:	4c                   	rex.WR
  c4:	45 5f                	rex.RB pop r15
  c6:	70 6c                	jo     134 <_init-0x3bc>
  c8:	75 73                	jne    13d <_init-0x3b3>
  ca:	00 5f 70             	add    BYTE PTR [rdi+0x70],bl
  cd:	6f                   	outs   dx,DWORD PTR ds:[rsi]
  ce:	73 00                	jae    d0 <_init-0x420>
  d0:	5f                   	pop    rdi
  d1:	73 62                	jae    135 <_init-0x3bb>
  d3:	75 66                	jne    13b <_init-0x3b5>
  d5:	00 5f 49             	add    BYTE PTR [rdi+0x49],bl
  d8:	4f 5f                	rex.WRXB pop r15
  da:	46                   	rex.RX
  db:	49                   	rex.WB
  dc:	4c                   	rex.WR
  dd:	45 00 75 6e          	add    BYTE PTR [r13+0x6e],r14b
  e1:	73 69                	jae    14c <_init-0x3a4>
  e3:	67 6e                	outs   dx,BYTE PTR ds:[esi]
  e5:	65 64 20 63 68       	gs and BYTE PTR fs:[rbx+0x68],ah
  ea:	61                   	(bad)  
  eb:	72 00                	jb     ed <_init-0x403>
  ed:	61                   	(bad)  
  ee:	64 64 32 2e          	fs xor ch,BYTE PTR fs:[rsi]
  f2:	63 00                	movsxd eax,DWORD PTR [rax]
  f4:	5f                   	pop    rdi
  f5:	49                   	rex.WB
  f6:	4f 5f                	rex.WRXB pop r15
  f8:	32 5f 31             	xor    bl,BYTE PTR [rdi+0x31]
  fb:	5f                   	pop    rdi
  fc:	73 74                	jae    172 <_init-0x37e>
  fe:	64 69 6e 5f 00 5f 49 	imul   ebp,DWORD PTR fs:[rsi+0x5f],0x4f495f00
 105:	4f 
 106:	5f                   	pop    rdi
 107:	6d                   	ins    DWORD PTR es:[rdi],dx
 108:	61                   	(bad)  
 109:	72 6b                	jb     176 <_init-0x37a>
 10b:	65 72 00             	gs jb  10e <_init-0x3e2>
 10e:	5f                   	pop    rdi
 10f:	73 68                	jae    179 <_init-0x377>
 111:	6f                   	outs   dx,DWORD PTR ds:[rsi]
 112:	72 74                	jb     188 <_init-0x368>
 114:	62                   	(bad)  
 115:	75 66                	jne    17d <_init-0x373>
 117:	00 5f 49             	add    BYTE PTR [rdi+0x49],bl
 11a:	4f 5f                	rex.WRXB pop r15
 11c:	77 72                	ja     190 <_init-0x360>
 11e:	69 74 65 5f 62 61 73 	imul   esi,DWORD PTR [rbp+riz*2+0x5f],0x65736162
 125:	65 
 126:	00 5f 75             	add    BYTE PTR [rdi+0x75],bl
 129:	6e                   	outs   dx,BYTE PTR ds:[rsi]
 12a:	75 73                	jne    19f <_init-0x351>
 12c:	65 64 32 00          	gs xor al,BYTE PTR fs:[rax]
 130:	5f                   	pop    rdi
 131:	49                   	rex.WB
 132:	4f 5f                	rex.WRXB pop r15
 134:	72 65                	jb     19b <_init-0x355>
 136:	61                   	(bad)  
 137:	64 5f                	fs pop rdi
 139:	70 74                	jo     1af <_init-0x341>
 13b:	72 00                	jb     13d <_init-0x3b3>
 13d:	73 68                	jae    1a7 <_init-0x349>
 13f:	6f                   	outs   dx,DWORD PTR ds:[rsi]
 140:	72 74                	jb     1b6 <_init-0x33a>
 142:	20 75 6e             	and    BYTE PTR [rbp+0x6e],dh
 145:	73 69                	jae    1b0 <_init-0x340>
 147:	67 6e                	outs   dx,BYTE PTR ds:[esi]
 149:	65 64 20 69 6e       	gs and BYTE PTR fs:[rcx+0x6e],ch
 14e:	74 00                	je     150 <_init-0x3a0>
 150:	6d                   	ins    DWORD PTR es:[rdi],dx
 151:	61                   	(bad)  
 152:	69 6e 00 5f 6e 65 78 	imul   ebp,DWORD PTR [rsi+0x0],0x78656e5f
 159:	74 00                	je     15b <_init-0x395>
 15b:	5f                   	pop    rdi
 15c:	5f                   	pop    rdi
 15d:	70 61                	jo     1c0 <_init-0x330>
 15f:	64 31 00             	xor    DWORD PTR fs:[rax],eax
 162:	5f                   	pop    rdi
 163:	5f                   	pop    rdi
 164:	70 61                	jo     1c7 <_init-0x329>
 166:	64 32 00             	xor    al,BYTE PTR fs:[rax]
 169:	5f                   	pop    rdi
 16a:	5f                   	pop    rdi
 16b:	70 61                	jo     1ce <_init-0x322>
 16d:	64 33 00             	xor    eax,DWORD PTR fs:[rax]
 170:	5f                   	pop    rdi
 171:	5f                   	pop    rdi
 172:	70 61                	jo     1d5 <_init-0x31b>
 174:	64 34 00             	fs xor al,0x0
 177:	5f                   	pop    rdi
 178:	5f                   	pop    rdi
 179:	70 61                	jo     1dc <_init-0x314>
 17b:	64 35 00 6c 6f 6e    	fs xor eax,0x6e6f6c00
 181:	67 20 75 6e          	and    BYTE PTR [ebp+0x6e],dh
 185:	73 69                	jae    1f0 <_init-0x300>
 187:	67 6e                	outs   dx,BYTE PTR ds:[esi]
 189:	65 64 20 69 6e       	gs and BYTE PTR fs:[rcx+0x6e],ch
 18e:	74 00                	je     190 <_init-0x360>
 190:	5f                   	pop    rdi
 191:	49                   	rex.WB
 192:	4f 5f                	rex.WRXB pop r15
 194:	77 72                	ja     208 <_init-0x2e8>
 196:	69 74 65 5f 65 6e 64 	imul   esi,DWORD PTR [rbp+riz*2+0x5f],0x646e65
 19d:	00 
 19e:	5f                   	pop    rdi
 19f:	5f                   	pop    rdi
 1a0:	6f                   	outs   dx,DWORD PTR ds:[rsi]
 1a1:	66 66 36 34 5f       	data16 data16 ss xor al,0x5f
 1a6:	74 00                	je     1a8 <_init-0x348>
 1a8:	5f                   	pop    rdi
 1a9:	5f                   	pop    rdi
 1aa:	6f                   	outs   dx,DWORD PTR ds:[rsi]
 1ab:	66 66 5f             	data16 pop di
 1ae:	74 00                	je     1b0 <_init-0x340>
 1b0:	5f                   	pop    rdi
 1b1:	63 68 61             	movsxd ebp,DWORD PTR [rax+0x61]
 1b4:	69 6e 00 47 4e 55 20 	imul   ebp,DWORD PTR [rsi+0x0],0x20554e47
 1bb:	43 31 31             	rex.XB xor DWORD PTR [r9],esi
 1be:	20 37                	and    BYTE PTR [rdi],dh
 1c0:	2e 35 2e 30 20 2d    	cs xor eax,0x2d20302e
 1c6:	6d                   	ins    DWORD PTR es:[rdi],dx
 1c7:	74 75                	je     23e <_init-0x2b2>
 1c9:	6e                   	outs   dx,BYTE PTR ds:[rsi]
 1ca:	65 3d 67 65 6e 65    	gs cmp eax,0x656e6567
 1d0:	72 69                	jb     23b <_init-0x2b5>
 1d2:	63 20                	movsxd esp,DWORD PTR [rax]
 1d4:	2d 6d 61 72 63       	sub    eax,0x6372616d
 1d9:	68 3d 78 38 36       	push   0x3638783d
 1de:	2d 36 34 20 2d       	sub    eax,0x2d203436
 1e3:	67 20 2d 66 73 74 61 	and    BYTE PTR [eip+0x61747366],ch        # 61747550 <_end+0x61546538>
 1ea:	63 6b 2d             	movsxd ebp,DWORD PTR [rbx+0x2d]
 1ed:	70 72                	jo     261 <_init-0x28f>
 1ef:	6f                   	outs   dx,DWORD PTR ds:[rsi]
 1f0:	74 65                	je     257 <_init-0x299>
 1f2:	63 74 6f 72          	movsxd esi,DWORD PTR [rdi+rbp*2+0x72]
 1f6:	2d 73 74 72 6f       	sub    eax,0x6f727473
 1fb:	6e                   	outs   dx,BYTE PTR ds:[rsi]
 1fc:	67 00 5f 49          	add    BYTE PTR [edi+0x49],bl
 200:	4f 5f                	rex.WRXB pop r15
 202:	62 61                	(bad)  
 204:	63 6b 75             	movsxd ebp,DWORD PTR [rbx+0x75]
 207:	70 5f                	jo     268 <_init-0x288>
 209:	62 61                	(bad)  
 20b:	73 65                	jae    272 <_init-0x27e>
 20d:	00 73 74             	add    BYTE PTR [rbx+0x74],dh
 210:	64 69 6e 00 5f 66 6c 	imul   ebp,DWORD PTR fs:[rsi+0x0],0x616c665f
 217:	61 
 218:	67 73 32             	addr32 jae 24d <_init-0x2a3>
 21b:	00 5f 6d             	add    BYTE PTR [rdi+0x6d],bl
 21e:	6f                   	outs   dx,DWORD PTR ds:[rsi]
 21f:	64 65 00 5f 49       	fs add BYTE PTR gs:[rdi+0x49],bl
 224:	4f 5f                	rex.WRXB pop r15
 226:	72 65                	jb     28d <_init-0x263>
 228:	61                   	(bad)  
 229:	64 5f                	fs pop rdi
 22b:	62 61                	(bad)  
 22d:	73 65                	jae    294 <_init-0x25c>
 22f:	00 5f 76             	add    BYTE PTR [rdi+0x76],bl
 232:	74 61                	je     295 <_init-0x25b>
 234:	62                   	(bad)  
 235:	6c                   	ins    BYTE PTR es:[rdi],dx
 236:	65 5f                	gs pop rdi
 238:	6f                   	outs   dx,DWORD PTR ds:[rsi]
 239:	66 66 73 65          	data16 data16 jae 2a2 <_init-0x24e>
 23d:	74 00                	je     23f <_init-0x2b1>
 23f:	5f                   	pop    rdi
 240:	49                   	rex.WB
 241:	4f 5f                	rex.WRXB pop r15
 243:	73 61                	jae    2a6 <_init-0x24a>
 245:	76 65                	jbe    2ac <_init-0x244>
 247:	5f                   	pop    rdi
 248:	62 61                	(bad)  
 24a:	73 65                	jae    2b1 <_init-0x23f>
 24c:	00 73 79             	add    BYTE PTR [rbx+0x79],dh
 24f:	73 5f                	jae    2b0 <_init-0x240>
 251:	65 72 72             	gs jb  2c6 <_init-0x22a>
 254:	6c                   	ins    BYTE PTR es:[rdi],dx
 255:	69 73 74 00 5f 66 69 	imul   esi,DWORD PTR [rbx+0x74],0x69665f00
 25c:	6c                   	ins    BYTE PTR es:[rdi],dx
 25d:	65 6e                	outs   dx,BYTE PTR gs:[rsi]
 25f:	6f                   	outs   dx,DWORD PTR ds:[rsi]
 260:	00 73 74             	add    BYTE PTR [rbx+0x74],dh
 263:	64 6f                	outs   dx,DWORD PTR fs:[rsi]
 265:	75 74                	jne    2db <_init-0x215>
 267:	00 5f 49             	add    BYTE PTR [rdi+0x49],bl
 26a:	4f 5f                	rex.WRXB pop r15
 26c:	32 5f 31             	xor    bl,BYTE PTR [rdi+0x31]
 26f:	5f                   	pop    rdi
 270:	73 74                	jae    2e6 <_init-0x20a>
 272:	64 6f                	outs   dx,DWORD PTR fs:[rsi]
 274:	75 74                	jne    2ea <_init-0x206>
 276:	5f                   	pop    rdi
 277:	00 5f 49             	add    BYTE PTR [rdi+0x49],bl
 27a:	4f 5f                	rex.WRXB pop r15
 27c:	6c                   	ins    BYTE PTR es:[rdi],dx
 27d:	6f                   	outs   dx,DWORD PTR ds:[rsi]
 27e:	63 6b 5f             	movsxd ebp,DWORD PTR [rbx+0x5
```
