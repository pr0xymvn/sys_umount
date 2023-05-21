BITS 64

global _umount

section .rodata
	success db "/mnt Unmount with success :)", 10, 0
	file_umount db "/mnt", 0

section .text

_umount:
	mov rax, 166
	mov rdi, file_umount
	mov rsi, 02
	syscall
	jmp _exit

_exit:
	mov rax, 0x3C
	mov rdi, 0	
	syscall
