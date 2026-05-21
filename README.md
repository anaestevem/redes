# redes TOPOLOGIA DE REDE

ESTRELA
Todos os dispositivos (computadores, impressoras, servidores) conectam-se individualmente a um nó central (geralmente um switch ou roteador) é uma estrutura de rede em que cada dispositivo e ponto de conexão estão conectados a um hub central.

CARACTERÍSTICAS E DIFERENÇAS
Conexão Direta: Cada dispositivo (computador, impressora, servidor) tem seu próprio cabo conectado individualmente ao equipamento central. A comunicação vai para o centro e é redirecionada.
Impacto de Falhas: Se um cabo se romper ou um computador apresentar defeito, a falha é isolada e apenas aquele dispositivo fica sem conexão. Por outro lado, se o dispositivo central parar de funcionar, toda a rede fica inoperante.
Escalabilidade Simples: Adicionar novos computadores é fácil e não interrompe o funcionamento da rede; basta plugar o cabo em uma porta livre do concentrador.
Uso de Cabeamento: Exige uma quantidade significativamente maior de cabos em comparação com outras topologias (como anel ou barramento), o que pode elevar os custos de instalação.

USO NO DIA A DIA
Todos os dispositivos (computadores, impressoras, TVs) se conectam a um ponto central, geralmente um switch ou roteador.
Em casa (Rede Doméstica): O seu roteador Wi-Fi central atua como o ponto focal. Seus celulares, notebooks e smart TVs conectam-se a ele. Se a TV perder o sinal, seu notebook continua navegando na internet sem problemas.
Em escritórios e empresas: Vários computadores e impressoras são conectados via cabos de rede a um switch central, que por sua vez liga a rede à internet. Isso facilita a expansão da rede: basta plugar um novo aparelho na porta vazia do switch.
Câmeras de Segurança (CFTV): Sistemas modernos de monitoramento IP usam switches para centralizar as imagens de todas as câmeras em um único gravador ou computador.
ANEL
Conecta dispositivos em um circuito fechado, onde os dados viajam de forma sequencial, passando de um computador para o outro. 

CARACTERÍSTICAS E DIFERENÇAS
Fluxo de Dados: Unidirecional (na maioria das vezes), seguindo um sentido horário ou anti-horário.
Acesso Token: Muitas redes em anel usam um token (testemunha), um pacote de dados que circula na rede. Só pode transmitir quem detém o token, evitando colisões.
Expansão: Adicionar ou remover um computador exige a quebra do anel, parando temporariamente o tráfego.
Funcionamento: Cada equipamento atua como um repetidor de sinal, passando as informações para o vizinho até chegar ao destinatário. Os dados circulam em uma ou ambas as direções (anel duplo).
Vantagens: Facilidade para expandir a rede e eficiência no tráfego pesado de dados.
Desvantagens: Na sua forma básica, a falha de um único computador pode derrubar toda a rede.
Diferenças para Outras Topologias:Comparar o modelo em anel com outras arquiteturas ajuda a entender sua viabilidade.

USO NO DIA A DIA
De fibra Automação Industrial: Muito utilizada para conectar sensores e equipamentos pesados (CLPs) em fábricas. A estrutura em anel permite que, se um cabo romper, os dados façam o caminho inverso, evitando a parada de toda a produção.
Provedores de Internet: Em menor escala, os provedores utilizam essa topologia para interligar centrais. Se uma rota óptica for cortada acidentalmente, o tráfego é redirecionado pelo outro lado do anel, mantendo a sua internet funcionando.


MALHA
É uma configuração de rede onde cada dispositivo (nó) se conecta diretamente a vários ou a todos os outros equipamentos. 

CARACTERÍSTICAS E DIFERENÇAS
Alta Confiabilidade: Se uma conexão ou cabo se romper, os dados encontram outro caminho de forma automática.
Desempenho Estável: Como os links são dedicados, não há congestionamento por disputa de canais.
Altos Custos: Demanda mais cabos, portas de rede e equipamentos, tornando sua implementação cabeada muito cara.
Aplicações Práticas: Muito aplicada em redes corporativas de grande porte (data centers), conexões backbone (espinha dorsal) da internet e, hoje em dia, em redes sem fio (Wireless Mesh Networks).
DOIS TIPOS
Malha Completa: Todos os dispositivos estão interligados entre si. Oferece a maior redundância possível, mas exige grande quantidade de cabos e possui custo muito alto.
Malha Parcial: Apenas os dispositivos que mais se comunicam ou os nós críticos estão interligados. É a variação mais comum no mundo corporativo e em provedores, pois equilibra a tolerância a falhas com a redução de custos
Sua principal diferença para as topologias tradicionais (como Estrela ou Barramento) é a alta redundância e resiliência, já que não depende de um único ponto central para funcionar.
USO NO DIA A DIA
Wi-Fi Residencial e Comercial: Sistemas de Redes Mesh substituem repetidores tradicionais. Eles criam uma única rede que "cola" os dispositivos móveis ao melhor ponto disponível enquanto você caminha pelo ambiente.
Cidades Inteligentes: Utilizada para manter a comunicação de câmeras de segurança e sensores de tráfego em áreas amplas, permitindo que os dados façam desvios automáticos caso um caminho esteja congestionado ou fora do ar.
Infraestrutura Crítica: Em data centers e grandes empresas, garante que, caso um cabo rompa ou um roteador pare de funcionar, os dados encontrem rotas alternativas para chegar ao destino instantaneamente.
BARRAMENTO
Conecta todos os dispositivos (nós) a um único cabo central compartilhado, conhecido como backbone ou espinha dorsal. 
CARACTERÍSTICAS E DIFERENÇAS
Estrutura Linear: Todos os nós (computadores, impressoras) são ligados diretamente a um cabo principal.
Comunicação Compartilhada: Os dados enviados por um dispositivo são transmitidos para toda a rede. Cada nó verifica a informação, mas apenas o destinatário correto a processa.
Transmissão Half-Duplex: Como o canal é compartilhado, apenas um dispositivo pode transmitir dados por vez. Se dois enviarem sinais simultaneamente, ocorre uma colisão e a transmissão precisa ser reiniciada.
Terminadores: As extremidades do cabo principal possuem "terminadores". Eles absorvem os sinais elétricos, impedindo que as informações fiquem rebatendo e circulando infinitamente pela rede.
Fácil Instalação: Exige uma quantidade significativamente menor de cabos comparada a outras topologias, como a estrela.
Vantagens:Custo mais baixo de implementação devido à menor metragem de cabo. Fácil instalação e expansão.
Desvantagens:O rompimento do cabo principal paralisa todos os dispositivos da rede. Como a via é compartilhada, se duas máquinas enviarem dados juntas.
A grande diferença para outras redes é sua simplicidade e vulnerabilidade, se o cabo central romper, a rede inteira para, e apenas um computador pode transmitir dados por vez para
USO NO DIA A DIA📍
Automação Industrial e IoT: Muito utilizada em fábricas e painéis de controle, onde sensores ou CLPs (Controladores Lógicos Programáveis) são ligados em uma mesma linha.
Provedores de Internet (Fibra Óptica - GPON): Na infraestrutura de distribuição de internet, o sinal sai de um ponto central e é dividido para vários clientes usando uma estrutura linear.
