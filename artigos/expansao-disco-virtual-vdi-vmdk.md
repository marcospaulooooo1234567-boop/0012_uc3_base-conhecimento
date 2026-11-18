# Expansão de Disco Virtual VDI e VMDK

## 1. Introdução
Máquinas virtuais utilizam discos virtuais para armazenar arquivos, programas e sistemas operacionais. Quando o espaço acaba, é necessário aumentar sua capacidade.

## 2. Identificação do problema
A falta de espaço pode impedir a instalação de programas e o salvamento de arquivos. Antes de alterar o disco, faça um backup da máquina virtual.

## 3. Expansão de disco VDI no VirtualBox
1. Desligue a máquina virtual.
2. Abra o Prompt de Comando do Windows.
3. Execute: `VBoxManage modifymedium disk "C:\caminho\disco.vdi" --resize 51200`.
4. O valor 51200 representa aproximadamente 50 GB.
5. Inicie a máquina e amplie a partição pelo gerenciamento de disco.

## 4. Expansão de disco VMDK no VMware
1. Desligue a máquina virtual.
2. Abra o VMware Workstation.
3. Acesse as configurações da máquina virtual.
4. Selecione o disco rígido e utilize a opção Expand.
5. Inicie a máquina e amplie a partição pelo sistema operacional.

## 5. Cuidados importantes
- Faça backup antes de qualquer alteração.
- Verifique se existe espaço disponível no disco físico.
- Nunca expanda o disco com a máquina virtual ligada.
- Confira se a partição também foi ampliada.

## 6. Conclusão
A expansão de discos VDI e VMDK permite aumentar o armazenamento das máquinas virtuais. Seguindo os procedimentos corretos, é possível resolver problemas de falta de espaço com segurança.