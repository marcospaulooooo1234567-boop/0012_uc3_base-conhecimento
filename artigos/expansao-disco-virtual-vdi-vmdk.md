# Como expandir um disco virtual VDI e VMDK

## 1. Introdução

As máquinas virtuais utilizam discos virtuais para armazenar arquivos, programas e sistemas operacionais. Com o tempo, esses discos podem ficar sem espaço, causando dificuldades no funcionamento da máquina virtual.

Este artigo apresenta como expandir discos virtuais VDI, utilizados pelo Oracle VirtualBox, e VMDK, utilizados pelo VMware Workstation.

## 2. Identificando o problema

Quando o disco virtual fica cheio, o sistema operacional pode apresentar mensagens de falta de espaço, impedir a instalação de programas e dificultar o salvamento de arquivos.

Antes de realizar qualquer alteração, é importante fazer um backup da máquina virtual.

## 3. Expandindo disco VDI no VirtualBox

1. Desligue completamente a máquina virtual.
2. Abra o Prompt de Comando do Windows.
3. Localize o arquivo VDI da máquina virtual.
4. Execute o comando de redimensionamento:

```bash
VBoxManage modifymedium disk "C:\caminho\disco.vdi" --resize 51200
```

O valor 51200 representa aproximadamente 50 GB.

5. Abra a máquina virtual e utilize o gerenciamento de disco do sistema operacional para ampliar a partição.

## 4. Expandindo disco VMDK no VMware

1. Desligue a máquina virtual.
2. Abra o VMware Workstation.
3. Selecione a máquina virtual desejada.
4. Acesse as configurações da máquina virtual.
5. Selecione o disco rígido virtual.
6. Utilize a opção Expand para aumentar a capacidade do disco.
7. Inicie a máquina virtual e amplie a partição pelo sistema operacional.

## 5. Cuidados importantes

- Faça backup antes de alterar o disco.
- Nunca expanda um disco com a máquina virtual ligada.
- Verifique se existe espaço disponível no disco físico.
- Confira se a partição do sistema operacional também foi ampliada.

## 6. Conclusão

A expansão de discos virtuais VDI e VMDK é uma solução importante quando uma máquina virtual fica sem espaço. Seguindo os procedimentos corretos e realizando backups, é possível aumentar a capacidade de armazenamento e melhorar o funcionamento da máquina virtual.