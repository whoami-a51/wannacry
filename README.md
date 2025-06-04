O WannaCry é um dos ransomwares mais famosos da história da cibersegurança. Ele foi responsável por um ataque global em maio de 2017, criptografando mais de 200 mil computadores em 150 países.

![descrição](/imgs/wannacry.png)


🧨 O que o WannaCry fazia?

Ele criptografava os arquivos do computador da vítima e exibia uma mensagem exigindo um resgate em Bitcoin para descriptografá-los. A tela tinha um cronômetro, e se o pagamento não fosse feito a tempo, os arquivos seriam perdidos para sempre.
🧠 Como ele funcionava?

O WannaCry se aproveitou de uma vulnerabilidade crítica no Windows, chamada EternalBlue, que foi desenvolvida pela NSA (Agência de Segurança Nacional dos EUA) e vazada pelo grupo Shadow Brokers.

Essa falha permitia execução remota de código no protocolo SMB (Server Message Block), usado para compartilhamento de arquivos em redes Windows.

Em resumo:
 1. Ele explorava a falha SMBv1 para se infiltrar.
 2. Se propagava automaticamente em redes internas (worm).
 3. Criptografava tudo e cobrava resgate.

🏥 Quem foi afetado?
 • Hospitais britânicos (NHS): cancelaram cirurgias, perderam acesso a registros médicos.
 • Renault, Nissan: fábricas paralisadas.
 • FedEx, Telefónica, universidades na China.
 • Até caixas eletrônicos travaram em alguns lugares.

🔐 Como foi contido?

Um pesquisador conhecido como MalwareTech descobriu um “kill switch” embutido no malware: o WannaCry tentava se conectar a um domínio aleatório, e se tivesse resposta, parava. O pesquisador registrou esse domínio — e isso interrompeu boa parte do ataque.

O acesso remoto aos computadores para a execução do WannaCry foi feito atráves da vulnerabilidade no SMB1 - vazada da NSA - e uso do exploit Eternablue.

![descrição](/imgs/eternablue.png)


🧬 Curiosidades Técnicas
 • Linguagem: O dropper principal do WannaCry era escrito em C e C++.
 • Criptografia usada: RSA + AES.
 • Porta usada para se propagar: TCP 445 (SMB).
 • A Microsoft lançou um patch antes do ataque, mas muitos sistemas (principalmente Windows XP e Windows 7) não estavam atualizados.
