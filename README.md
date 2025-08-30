# Beneficios-da-Nuvem
desafio DIO: Criando a Primeira Máquina Virtual na Azure
Este repositório documenta a execução e os aprendizados do laboratório prático "Criando sua Primeira Máquina Virtual na Azure", parte do bootcamp da DIO. O objetivo deste desafio foi consolidar o conhecimento sobre um dos serviços de computação mais fundamentais da nuvem, aplicando os conceitos em um ambiente real e documentando o processo de forma clara e estruturada.

O Processo: Passo a Passo da Criação da VM
A criação de uma Máquina Virtual (VM) no portal da Azure é um processo estruturado que envolve a configuração de diversos recursos essenciais. Abaixo, descrevo as etapas principais que segui durante o laboratório:

Seleção do Serviço: No portal do Azure, naveguei até a categoria Computação e selecionei o serviço de Máquinas Virtuais.

Configuração Básica: Preenchi as informações essenciais da VM, como:

Grupo de Recursos: Um contêiner lógico para agrupar os recursos da Azure.

Nome da VM: Um nome único para identificar a máquina.

Região: O data center geográfico onde a VM será hospedada.

Imagem: O sistema operacional a ser instalado (ex: Windows Server, Ubuntu).

Tamanho: A configuração de hardware (CPU, RAM, Armazenamento) da VM, que impacta diretamente o custo e o desempenho.

Configuração de Rede e Discos: Defini as configurações de Rede Virtual (VNet) e as opções de disco de armazenamento para o sistema operacional.

Revisão e Criação: Após revisar todas as configurações para garantir que estavam corretas, finalizei o processo de criação. A Azure então realizou o provisionamento da VM, deixando-a pronta para uso.

Conceitos-Chave Aprofundados
Além do passo a passo prático, o laboratório aprofundou conceitos cruciais para a utilização profissional da Azure:

1. Service Level Agreement (SLA) - O Compromisso da Microsoft
Um dos conceitos mais importantes que aprendi foi o SLA (Service Level Agreement). Entendi que este é um compromisso formal da Microsoft sobre a garantia de tempo de atividade (uptime) de um serviço.

Garantia de Uptime: Cada serviço da Azure possui um SLA específico (ex: 99,9%, 99,99%).

Crédito por Inatividade: Caso a Microsoft não cumpra o tempo de atividade prometido no SLA, a empresa reembolsa o cliente com créditos de serviço.

Variação do SLA: O percentual do SLA pode variar drasticamente dependendo do serviço e, crucialmente, da configuração de redundância escolhida.

2. Contas de Armazenamento e Redundância de Dados
A escolha correta da redundância de dados é fundamental, pois impacta diretamente o custo e o nível de SLA da aplicação.

As principais opções que explorei foram:

LRS (Locally-Redundant Storage): A opção mais barata. Replica os dados três vezes dentro de um único data center. Protege contra falhas de hardware, mas não contra um desastre que afete o data center inteiro.

ZRS (Zone-Redundant Storage): Replica os dados entre três "zonas de disponibilidade" (data centers distintos) dentro da mesma região. Oferece uma proteção muito maior que o LRS.

GRS (Geo-Redundant Storage): Replica os dados para uma segunda região, a centenas de quilômetros de distância, protegendo contra desastres regionais.

GZRS (Geo-Zone-Redundant Storage): A opção mais robusta e cara. Combina a redundância de zona (ZRS) na região primária com a replicação geográfica (GRS) para uma segunda região.

3. Navegação e Documentação Integrada
A experiência no portal reforçou a facilidade de uso da plataforma. Cada item de configuração possui um breve resumo explicativo e um link "Saiba mais", que direciona para a documentação oficial da Microsoft. Isso torna o aprendizado contínuo e a consulta a detalhes técnicos um processo integrado e muito eficiente.

🏁 Conclusão
Este laboratório foi extremamente valioso para materializar os conceitos teóricos da computação em nuvem. Criar uma Máquina Virtual na prática, e entender como decisões de configuração — como as opções de redundância de armazenamento — afetam diretamente o custo e a resiliência (SLA) de uma solução, são conhecimentos fundamentais. Sinto-me mais confiante para provisionar e gerenciar recursos de computação na Azure.
