G7 Plus XT1965-2 (lake) - builder batteryless para LineageOS 22.2

Este pacote NÃO é para flash direto.
Ele cria um kernel de teste no GitHub Actions.

O patch faz 3 coisas:
1) mantém a detecção BMD (battery missing) desativada no PM660;
2) ignora a IRQ BT_MISS sem invalidar o perfil/SOC;
3) usa SB18C44559 (JG40-2) como perfil padrão quando o bootloader não fornece mmi,battid.

Depois que o GitHub Actions terminar, baixe o artifact:
  g7plus-lake-batteryless-kernel

O arquivo importante será:
  Image.gz-dtb

NÃO grave Image.gz-dtb diretamente no celular.
Envie o artifact para o ChatGPT. Ele será inserido no boot.img correto da sua build 22.2.
