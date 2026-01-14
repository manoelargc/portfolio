UI4DEVS: UMMVPPARAAPOIARDESENVOLVEDORES NACRIAÇÃO DE
INTERFACES
Manoela Resende†
Prof. Dr. Maicon Bernardinoß
RESUMO
Desenvolvedores frequentemente assumem responsabilidades de interface sem do-
mínio dos fundamentos de design, o que resulta em sistemas com falhas de usabi-
lidade e inconsistências visuais. A partir da análise de padrões recorrentes obser-
vados em avaliações aplicadas a diferentes contextos de interface, estruturou-se um
conjunto de recomendações que deu origem ao UI4Devs, um guia prático destinado
a orientar decisões de UI no cotidiano de equipes técnicas. Com base nesses funda-
mentos, foi desenvolvido um Produto Mínimo Viável que traduz as diretrizes do guia
em etapas guiadas, exemplos visuais e atividades aplicáveis. O MVP foi então sub-
metido a um processo de validação por meio de umsurvey, no qual participantes
exploraram o aplicativo e relataram suas primeiras impressões sobre clareza, aplica-
bilidade e utilidade prática. Os resultados indicaram que o modelo interativo facilita
a compreensão de conceitos de UI, apoia decisões visuais com maior segurança e
reduz dificuldades enfrentadas por desenvolvedores. As evidências reforçam o po-
tencial do UI4Devs como ferramenta de apoio para aprimorar interfaces, ampliar boas
práticas em equipes técnicas e democratizar princípios essenciais de usabilidade.
Palavras-chaves:Guia prático; Interface do usuário (UI); Ferramenta web; Usabili-
dade; Desenvolvedores.
ABSTRACT
Developers often take on interface-related responsibilities without a solid foundation
in design principles, which leads to systems that exhibit usability issues and visual
inconsistencies. From the analysis of recurring patterns identified in multiple interface
evaluations, a set of practical recommendations was consolidated and became the
foundation of UI4Devs, a guide designed to support UI decision, making within tech-
nical teams. Building on these insights, an interactive Minimal Viable Product (MVP)
was developed to translate the guide’s principles into guided steps, visual examples,
and hands-on activities. The MVP was then evaluated through a survey in which par-
ticipants explored the application and shared their first impressions regarding clarity,
applicability, and practical usefulness. The results indicate that the interactive format
enhances the understanding of UI concepts, supports more confident visual decision-
making, and alleviates common challenges faced by developers. Overall, the findings
highlight the potential of UI4Devs as a supportive tool for improving interface quality,
strengthening good practices within technical teams, and promoting wider adoption of
essential usability principles.
Keywords:Pratical guide; User interface (UI); Web tool; usability; Developers.
†Aluna do Curso de Ciência da Computação da Universidade Federal do Pampa, Alegrete, Rio Grande do Sul, Brasil
E-mail: manoelacunha.aluno@unipampa.edu.br
ßOrientador, Professor do Curso de Ciência da Computação da Universidade Federal do Pampa, Alegrete, Rio Grande do Sul,
Brasil, E-mail: bernardino@unipampa.edu.br

1. INTRODUÇÃO
Nas organizações de desenvolvimento de software, observa-se frequentemente
que programadores e equipes técnicas dispõem de conhecimentos robustos em ló-
gica, arquitetura de sistemas eframeworks, mas carecem de fundamentos consolida-
dos emUI/UX (User Interface and User Experience)(NIELSEN, 1994a; GARRETT,
2002). Essa lacuna leva à criação de interfaces que, embora funcionais, apresentam
falhas de legibilidade, problemas de navegação, ausência defeedbackadequado e
inconsistências visuais, comprometendo significativamente a experiência do usuário
e afetando a adoção e o sucesso das aplicações (NIELSEN, 1994a).
Esse cenário é agravado por dados que evidenciam a prevalência de práticas
que não aderem às recomendações internacionais de acessibilidade. Estimativas
indicam que a falta de acessibilidade em canais digitais pode gerar perdas financei-
ras expressivas, como apontado por relatório da revistaForbes, que estima prejuízos
globais anuais de até 16 bilhões de dólares decorrentes de interfaces inacessíveis
(ALEXIOU, 2021). A pesquisa anual da WebAIM reforça esse quadro ao apontar que
apenas 3,7% das páginas iniciais dos principais sites do mundo são plenamente aces-
síveis, revelando a persistência de erros estruturais mesmo em soluções amplamente
difundidas (WebAIM, 2023).
Diante desse contexto, tornou-se necessário compreender como falhas recorren-
tes de usabilidade se manifestam em sistemas reais e como podem ser mitigadas por
meio de diretrizes práticas acessíveis a equipes sem especialização em design. A
análise sistemática de duas interfaces distintas permitiu identificar padrões de proble-
mas e consolidar um conjunto de recomendações que culminou na estruturação do
UI4Devs, um guia prático de interface voltado a desenvolvedores.
A etapa seguinte consistiu em transformar esse guia em uma aplicação interativa,
com o objetivo de torná-lo mais acessível, aplicável e alinhado ao fluxo de trabalho
de equipes técnicas. Para isso, foi desenvolvido umMínimo Produto Viável(MVP)
que organiza as recomendações em etapas guiadas, exemplos visuais, atividades
práticas e decisões parametrizadas. Essa versão inicial não apenas operacionaliza
as diretrizes do guia, mas também cria um ambiente de aprendizagem que facilita o
entendimento e a incorporação de boas práticas deUIno desenvolvimento cotidiano.
Com o MVP implementado, conduziu-se uma etapa de validação por meio de um
surveycomposto por duas fases: um formulário de pré-uso, destinado à caracteriza-
ção do público e ao levantamento de sua familiaridade com UI, e um formulário de
pós-uso, no qual os participantes testaram o aplicativo e registraram suas percep-
ções. A análise dos dados combinou abordagens quantitativas e qualitativas, per-
mitindo tanto mensurar tendências gerais quanto interpretar nuances presentes nos
relatos dos participantes. Durante a exploração do MVP , os usuários interagiram com
suas funcionalidades e avaliaram aspectos como clareza das etapas, utilidade prática
e aplicabilidade das recomendações. Esse processo forneceu evidências empíricas
sobre a eficácia do formato interativo e permitiu identificar contribuições e oportunida-
des de aprimoramento, fortalecendo a continuidade do projeto.
O objetivo geral deste estudo consiste em avaliar a eficácia de um MVP , derivado
do guia UI4Devs, em apoiar desenvolvedores na compreensão e aplicação de dire-
trizes práticas de interface. Para alcançar esse propósito, definem-se os seguintes
objetivos específicos:


OE1.Realizar a etapa preparatória que conecta o guia documentado à sua implemen-
tação, incluindo definição de requisitos, ajustes conceituais e organização do es-
copo do MVP;
OE2.Desenvolver um MVP que traduza as recomendações do guia em etapas claras,
aplicáveis e exemplos visuais;
OE3.Validar a clareza, a utilidade e a aplicabilidade da ferramenta junto ao público-alvo
por meio de umsurvey;
OE4.Analisar dados quantitativos e qualitativos referentes às percepções de compre-
ensão, aprendizado, aplicabilidade prática e facilidade de uso;
OE5.Produzir evidências que subsidiem a evolução futura do guia e da aplicação.
A partir desse conjunto de objetivos, a investigação central busca responder à
seguinte Questão de Pesquisa (QP):
QP:Como um guia prático fundamentado em erros reais de usabilidade e
integrado a um MVP pode apoiar desenvolvedores com diferentes níveis de
experiência na compreensão, análise e aplicação de boas práticas de interface
gráfica?
As contribuições desta pesquisa alcançam tanto o campo acadêmico quanto a
prática profissional, ao integrar diretrizes de usabilidade em uma ferramenta intera-
tiva, avaliar sua aplicabilidade por meio de experimentação direta e revelar padrões
reais de dificuldades enfrentadas por desenvolvedores. Ao incentivar a adoção de
princípios de design centrado no usuário, a investigação contribui para reduzir retra-
balho, elevar a maturidade visual de sistemas desenvolvidos por equipes técnicas e
ampliar o acesso a práticas qualificadas de UI.
Para orientar o percurso investigativo, apresenta-se inicialmente a fundamenta-
ção teórica que sustenta o estudo e os trabalhos relacionados, seguida das etapas
metodológicas adotadas no desenvolvimento do guia e na implementação do MVP . Na
sequência, são descritos o modelo interativo, as tecnologias utilizadas e o processo
de validação porsurvey. Por fim, discutem-se os resultados obtidos, suas implicações,
limitações e perspectivas para pesquisas futuras.
2. FUNDAMENTAÇÃOTEÓRICA
Esta seção reúne os conceitos e diretrizes que sustentam a análise e o desen-
volvimento deste trabalho, integrando conceitos essenciais da IHC, UI e UX, bem
como os principais referenciais utilizados nas avaliações: os princípios C.R.A.P ., as
heurísticas de Nielsen, os critérios da WCAG e as normas ISO relacionadas à usa-
bilidade. Esses elementos fornecem a base conceitual necessária para compreender
os aspectos visuais, funcionais e acessíveis das interfaces analisadas, estruturando
o entendimento que orienta tanto as avaliações conduzidas quanto a elaboração do
guia proposto.
2.1. INTERAÇÃOHUMANO–COMPUTADOR, UIEEXPERIÊNCIA DOUSUÁRIO
A Interação Humano–Computador (IHC) é o campo que investiga as formas pe-
las quais as pessoas interagem com sistemas computacionais, bem como os princí-
pios, técnicas e métodos empregados no projeto de sistemas interativos (BARBOSA;


SILVA, 2021). Como área multidisciplinar, a IHC combina conhecimentos da ciência
da computação, design, psicologia cognitiva e engenharia, buscando promover inte-
rações mais eficazes, acessíveis e agradáveis entre seres humanos e tecnologias
digitais.
Dentro desse campo, dois conceitos fundamentais se destacam: aUser Interface
(UI) e aUser Experience(UX). A UI refere-se aos elementos visuais, interativos e
operacionais que compõem a interface do sistema (como botões, menus, ícones e ti-
pografia), sendo responsável por estabelecer o canal de comunicação entre o usuário
e o sistema. Por outro lado, a UX envolve uma perspectiva mais ampla, que abrange
as emoções, percepções e respostas cognitivas dos usuários ao utilizar o sistema em
um determinado contexto (BARBOSA; SILVA, 2021), englobando também todos os
aspectos da interação do usuário final com a empresa, seus serviços e seus produtos
(NORMAN; NIELSEN, 2016).
A distinção entre UI e UX, embora frequentemente confundida, é essencial: en-
quanto a UI diz respeito à aparência e à operacionalidade da interface, a UX diz
respeito a como o usuário se sente ao interagir com o produto. Como afirma Barbosa
e Silva (2021), compreender essa diferenciação é crucial para desenvolver sistemas
mais eficazes, centrados nas pessoas, e capazes de gerar valor perceptível na vida
dos usuários.
2.2. PRINCÍPIOSC.R.A.P.
Os princípios de Contraste, Repetição, Alinhamento e Proximidade (C.R.A.P .),
apresentados por Williams (2012), fornecem diretrizes acessíveis e eficazes para a
organização visual de interfaces. Aplicações desses princípios contribuem para a cri-
ação de hierarquia informacional, coerência estética e maior clareza na composição
de elementos interativos.
Ainda que apresentados em formato didático e introdutório, esses princípios dia-
logam diretamente com noções consolidadas da psicologia da Gestalt, como as leis
da proximidade, similaridade e continuidade (KOFFKA, 1935). Essa relação reforça
a base perceptiva subjacente às escolhas visuais, mesmo quando apresentadas de
forma simplificada e pragmática.
No entanto, embora desempenhem um papel importante na formação básica em
design visual, tais princípios podem não atender integralmente às exigências de pro-
fissionais técnicos e desenvolvedores. Em contextos de alta demanda, com restrições
de tempo e recursos, há uma tendência à busca por diretrizes mais objetivas e direta-
mente aplicáveis ao cotidiano do desenvolvimento.
2.3. HEURÍSTICAS DEUSABILIDADE DENIELSEN
As heurísticas de Nielsen (NIELSEN, 1994a) constituem um conjunto consolidado
de dez princípios para identificar problemas comuns de usabilidade, como falta defe-
edback, inconsistências, sobrecarga cognitiva e dificuldade de recuperação de erros.
Utilizadas em inspeções heurísticas, permitem avaliar rapidamente a aderência de
uma interface a boas práticas de interação. Por serem diretrizes amplas e indepen-
dentes de tecnologia, aplicam-se tanto a sistemas web quanto a protótiposmobile-
first, auxiliando na priorização de melhorias com base na gravidade dos problemas
encontrados.


2.4. DIRETRIZES DEACESSIBILIDADE(WCAG 2.1E2.2)
AsWeb Content Accessibility Guidelines(WCAG 2.1 e 2.2) (W3C, 2023) esta-
belecem critérios para garantir que conteúdos digitais sejam Perceptíveis, Operáveis,
Compreensíveis e Robustos (POUR). Esses critérios orientam práticas como con-
traste adequado, navegação por teclado, textos claros, alternativas textuais e com-
patibilidade com tecnologias assistivas. A versão 2.2 introduz requisitos específicos
para navegação móvel, como área mínima de toque e maior previsibilidade de com-
portamento, essenciais em sistemas que priorizam a abordagemmobile-first.
2.5. NORMASISO RELACIONADAS ÀUSABILIDADE
A ISO 9241-11 (ISO, 2018) define usabilidade como a capacidade de um sistema
permitir que usuários atinjam objetivos com eficácia, eficiência e satisfação em deter-
minado contexto. Complementarmente, a ISO 9241-210 (ISO, 2019) orienta o design
centrado no usuário durante todo o ciclo de desenvolvimento, enfatizando a necessi-
dade de compreender os usuários, seus ambientes, tarefas e necessidades. Já a ISO
9241-110 (ISO, 2020) descreve princípios de interação, como consistência,feedback
informativo, controle do usuário e tolerância a erros.
Outras normas, como a ISO/IEC 25010 (ISO/IEC, 2011), acrescentam dimensões
de qualidade de software relacionadas à usabilidade, acessibilidade e experiência do
usuário, oferecendo uma base padronizada para avaliação e melhoria de interfaces.
Essas diretrizes não se limitam à camada visual e interativa das interfaces (UI),
mas abrangem também aspectos mais amplos da experiência do usuário (UX), ao
considerar fatores contextuais, emocionais e funcionais. Assim, as normas ISO con-
tribuem para alinhar práticas de design e desenvolvimento a princípios que integram
tanto a estrutura da interface quanto a vivência completa do usuário com o sistema.
3. TRABALHOSRELACIONADOS
Para fundamentar este estudo, realizamos umaRapid Review(CARTAXO; PINTO;
SOARES, 2020) da literatura, com foco em trabalhos aplicados e recentes. A busca
foi conduzida por meio do Google Scholar1, que integra diversas bases, como ACM
Digital Library, IEEE Xplore, SpringerLink e ScienceDirect. Combinamos palavras-
chave relacionadas à usabilidade, acessibilidade, design de interfaces e engenharia
de software, com ênfase em abordagens práticas, tais como guias eframeworksvol-
tados a equipes técnicas. Foram priorizados estudos publicados entre 2014 e 2025
que apresentassem contribuições metodológicas e aplicadas alinhadas aos objetivos
deste trabalho. Seis trabalhos representativos são sintetizados a seguir.
Costa e Canedo (2019) propuseram heurísticas refinadas de usabilidade voltadas
a aplicações móveis, adaptando os princípios clássicos de Nielsen às limitações de
telas reduzidas. A metodologia combinou avaliações heurísticas comfeedbackdireto
de usuários, demonstrando que aplicativos que seguem essas diretrizes apresentam
menos problemas críticos de usabilidade e maior satisfação geral. O trabalho destaca
a eficácia da adaptação heurística para apoiar desenvolvedores em contextos mobile.
Bakhshandeh (2025) investigou práticas de UI/UX inclusivas com foco na cons-
trução de experiências equitativas e acessíveis. Com base nos padrões da WCAG, o
1<https://scholar.google.com>


estudo revisou diretrizes organizacionais e realizou análises qualitativas de sua imple-
mentação. Os resultados revelaram lacunas persistentes entre a prática de mercado
e as recomendações de acessibilidade, reforçando a importância de integrar critérios
de acessibilidade desde as etapas iniciais do design, sobretudo para usuários com
deficiência.
Palomino et al. (2025) examinou como princípios de UI/UX afetam ferramentas
utilizadas por desenvolvedores, como IDEs eframeworksvisuais. Por meio de entre-
vistas com 25 desenvolvedores, inspeções heurísticas e análises observacionais, o
estudo demonstrou que ferramentas de desenvolvimento bem projetadas aumentam
a produtividade e reduzem a curva de aprendizado. Os resultados reforçam que até
mesmo sistemas voltados para uso técnico se beneficiam de padrões consistentes de
UI/UX, ampliando a discussão de usabilidade para além de aplicações finais.
Oswal (2014) analisou o papel do co-design participativo entre desenvolvedores e
especialistas em acessibilidade. A pesquisa utilizou oficinas participativas, prototipa-
ção rápida e avaliações com usuários com deficiência. Os achados confirmam que a
colaboração entre expertise técnica e de acessibilidade aumenta significativamente a
inclusividade em produtos finais. O estudo destaca o design participativo como uma
estratégia prática para elevar o nível de acessibilidade em projetos de desenvolvi-
mento.
Johnson (2020) investigou como desenvolvedores percebem seu papel nos pro-
cessos de UX. Com base em entrevistas qualitativas com 38 desenvolvedores, o es-
tudo identificou barreiras organizacionais e cognitivas para a colaboração com desig-
ners, incluindo ausência de formação, comunicação limitada e prioridades conflitan-
tes. O autor conclui que materiais práticos de capacitação e estruturas de colabora-
ção são essenciais para reduzir a distância entre desenvolvimento técnico e design
centrado no usuário.
Por fim, Mowar et al. (2025) apresentaram oCodeA11y, uma extensão para
GitHub Copilotprojetada para reforçar acessibilidade durante o desenvolvimento web.
A ferramenta integra verificações baseadas na WCAG diretamente em fluxos de codi-
ficação assistidos por IA, oferecendo sugestões de código sensíveis à acessibilidade,
lembretes para validações manuais e identificação automática de erros de conformi-
dade. Sua avaliação com desenvolvedores iniciantes mostrou melhorias na produção
de código acessível, embora o escopo permaneça limitado aos critérios da WCAG.
Em conjunto, os estudos analisados oferecem uma visão ampla sobre diretrizes
de usabilidade, acessibilidade e práticas colaborativas, explorando recortes especí-
ficos como heurísticas, critérios da WCAG ou abordagens participativas, como sin-
tetizado na Tabela 3. Embora relevantes, essas contribuições geralmente abordam
apenas uma dimensão do problema ou se limitam a análises conceituais. O pre-
sente estudo avança ao consolidar esses aportes em um guia prático estruturado, o
UI4Devs, e ao estender sua aplicação por meio de um MVP , validado com usuários.
A integração entre diretrizes consolidadas, implementação prática e validação empí-
rica distingue esta abordagem, oferecendo aos desenvolvedores um recurso acessí-
vel que combina fundamentação teórica, aplicação guiada e evidências coletadas em
contexto real de uso.


Tabela 1 - Comparação dos trabalhos relacionados.
Estudo Contribuição Público-alvo
Costa e Canedo
(2019)Heurísticas refinadas aplicáveis a dispositivos móveis Desenvolvedores mobile e avaliado-
res de UX
Bakhshandeh
(2025)Critérios de UX inclusiva alinhados à WCAG Equipes de design inclusivo
Palomino et al.
(2025)Análise do impacto de UI/UX em ferramentas para desenvolve-
doresDesenvolvedores técnicos
Oswal (2014) Abordagem de design participativo com especialistas em aces-
sibilidadeEquipes mistas de desenvolvimento
e acessibilidade
Johnson (2020) Barreiras encontradas na colaboração entre equipes de desen-
volvimento e UXDesenvolvedores de software
Mowar et al.
(2025)Assistente de IA com verificações automáticas baseadas na
WCAGDesenvolvedores web iniciantes
Este estudo Guia prático de UI, desenvolvimento de MVP e validação com
surveyDesenvolvedores sem formação em
design
4. METODOLOGIA
Este estudo está fundamentado no paradigma daDesign Science Research(DSR),
conforme proposto por Hevner e Chatterjee (2010), que orienta pesquisas voltadas à
concepção, construção e avaliação de artefatos destinados à resolução de proble-
mas práticos. Diferentemente de abordagens exclusivamente descritivas ou explicati-
vas, a DSR enfatiza a produção de soluções aplicáveis, sustentadas por rigor teórico
e validação empírica (GREGOR; JONES, 2007). Essa perspectiva é especialmente
adequada ao escopo deste trabalho, uma vez que a investigação não se limita à identi-
ficação de problemas de usabilidade, mas avança para o desenvolvimento e avaliação
de um artefato interativo (MVP) voltado ao apoio de desenvolvedores na aplicação de
boas práticas de UI.
Figura 1 - Estrutura metodológica da Design Science Research aplicada ao estudo,
baseada em Hevner e Chatterjee (2010).


Conforme apresentado na Figura 1, a metodologia do estudo articula três ciclos
centrais da Design Science Research. O ciclo da relevância conecta o problema in-
vestigado às necessidades reais do ambiente, representado por desenvolvedores,
estudantes de TI, freelancers e organizações com limitações em design de interface.
O ciclo do rigor assegura o embasamento teórico e metodológico da proposta, sus-
tentado por heurísticas de Nielsen, princípios C.R.A.P . e diretrizes WCAG. Já o ciclo
do design orienta a construção, refinamento e avaliação iterativa do artefato, materia-
lizado no guia prático de UI e em seu MVP interativo (UI4Devs).
Alinhada a esse paradigma, a pesquisa foi conduzida como um estudo científico
aplicado e estruturado, seguindo os princípios metodológicos descritos por Prodanov
e Freitas (2013). Seu propósito central consiste na geração de conhecimento com uso
prático imediato, especialmente no contexto do design e desenvolvimento de interfa-
ces digitais, materializado na proposta de um guia prático em formato de aplicação
interativa.
Quanto aos objetivos, a investigação apresenta caráter predominantemente ex-
ploratório e aplicado. As etapas anteriores do projeto permitiram identificar, classificar
e analisar problemas recorrentes de usabilidade e acessibilidade em sistemas reais,
resultando em um conjunto estruturado de diretrizes. Nesta etapa, o foco desloca-se
para a transformação dessas diretrizes em um produto funcional, investigando sua
clareza, utilidade e aderência às necessidades do público-alvo, em consonância com
o ciclo iterativo proposto pela DSR.
Do ponto de vista dos procedimentos técnicos, foram combinadas três estratégias
complementares. A análise documental forneceu a base teórica do estudo, contem-
plando heurísticas de Nielsen, princípios C.R.A.P ., diretrizes WCAG 2.2 e normas
internacionais relacionadas à usabilidade e acessibilidade. A etapa empírica, por sua
vez, deu origem ao mapeamento sistemático dos problemas de interface que funda-
mentaram a construção das diretrizes. A partir desse material, foram incorporadas
novas atividades, incluindo a modelagem conceitual do MVP (lean canvas, definição
de requisitos e arquitetura inicial), a implementação da aplicação interativa e sua pos-
terior validação por meio de um survey.
O delineamento metodológico adotou uma abordagem mista, integrando méto-
dos qualitativos e quantitativos. A análise qualitativa foi empregada para interpretar
aspectos subjetivos da interação com o MVP , como clareza das etapas, navegabili-
dade, adequação dos exemplos visuais e compreensibilidade das recomendações. A
análise quantitativa complementou essa interpretação, abrangendo métricas de uso,
recorrência de percepções nos questionários e avaliações de satisfação coletadas no
survey de pós-uso. Essa combinação permitiu compreender tanto a qualidade perce-
bida do artefato quanto sua efetividade prática.
Na construção das diretrizes que sustentam o MVP , foram aplicados três métodos
consolidados na área de Interação Humano-Computador: (i) análise visual orientada
pelos princípios C.R.A.P .; (ii) avaliação heurística baseada nas dez heurísticas de
Nielsen; (iii) verificação de conformidade com a WCAG 2.2, utilizando ferramentas au-
tomatizadas e inspeções manuais. Esses métodos asseguraram que o conteúdo do
guia estivesse fundamentado em evidências empíricas e critérios amplamente reco-
nhecidos.
A etapa atual do estudo adiciona ao processo a construção iterativa do artefato e


sua avaliação com usuários. A modelagem inicial envolveu a definição de requisitos
funcionais e não funcionais, o refinamento da estrutura dos módulos, a escolha das
tecnologias e a elaboração dos fluxos de interação. Após a implementação, o MVP
foi submetido a um processo de validação empírica por meio de um survey dividido
em momentos de pré-uso e pós-uso, no qual os participantes exploraram a aplicação
e relataram suas percepções quanto à clareza, aplicabilidade e utilidade das reco-
mendações. Esse ciclo de concepção, construção e avaliação reforça o alinhamento
do estudo ao paradigma da Design Science Research e sustenta a efetividade da
solução proposta.
5. AVALIAÇÃOINTEGRADA DASINTERFACES COMBASE EMC.R.A.P., NIELSEN E
WCAG
Esta seção apresenta uma avaliação integrada das interfaces dos sistemasRu-
bricProeOsiris, conduzida pela autora deste trabalho, com o objetivo de identificar
padrões recorrentes de problemas de usabilidade em contextos distintos de desen-
volvimento: um sistema real em uso institucional e um protótipomobile-firstem fase
de concepção. As análises aplicaram, de forma combinada, os princípios C.R.A.P .,
as heurísticas de Nielsen (1994a) e critérios selecionados da WCAG 2.2, comple-
mentados por ferramentas de apoio como SEER e Heurio para inspeção preliminar
e quadros estruturados no Figma para registro sistemático das evidências. Os pro-
blemas identificados foram posteriormente organizados segundo gravidade, recorrên-
cia e padrão, permitindo uma leitura comparativa consistente entre os dois sistemas.
Ressalta-se que não há qualquer vínculo prévio com as equipes responsáveis e com
os sistemas, assegurando neutralidade na observação, interpretação e registro das
evidências.
5.1. CARACTERIZAÇÃO DOSSISTEMAS
ORubricProé um sistema web utilizado por professores da UNIPAMPA para cria-
ção e aplicação de rubricas de avaliação. Desenvolvido por um único programador e
sem apoio especializado em design, representa um caso típico de interfaces produzi-
das por equipes essencialmente técnicas, nas quais decisões visuais e estruturais são
guiadas majoritariamente pela experiência prática. Como o sistema está diretamente
associado a processos de avaliação educacional, a clareza visual e a organização
das informações assumem papel central para a compreensão das rubricas e a fluidez
de uso.
OOsiris, por sua vez, evoluiu de um MVP inicialmente voltado ao aluguel de má-
quinas agrícolas para ummarketplacemais amplo. A nova versão foi prototipada por
uma equipe composta por quatro integrantes atuantes em programação e documen-
tação, também sem profissionais especializados em design de interfaces, caracteri-
zando um cenário comum em projetos técnicos e alinhado aos objetivos deste estudo.
A adoção de uma abordagemmobile-first(WROBLEWSKI, 2011) introduz demandas
específicas de layout, hierarquia e interação em dispositivos móveis, tornando a ava-
liação de usabilidade particularmente relevante na fase de prototipação.
A análise integrada desses dois sistemas, representando tanto um produto con-
solidado desenvolvido por um único programador quanto um protótipo elaborado por
uma equipe técnica, permite observar como padrões semelhantes de problemas emer-
gem independentemente do tamanho do time e da etapa do ciclo de desenvolvimento.


5.2. SÍNTESEINTEGRADA DOSRESULTADOS
Achados segundo C.R.A.P.:NoRubricPro, foram identificados 37 problemas,
concentrados sobretudo em desalinhamentos (43%), baixo contraste (21%), inconsis-
tência visual (19%) e falhas de proximidade (16%) (WILLIAMS, 2012). Esses aspec-
tos comprometiam a hierarquia das informações, a fluidez de leitura e a legibilidade
geral da interface. NoOsiris, foram registradas 39 ocorrências, sendo 19 distintas,
com destaque para problemas recorrentes de capitalização, ausência de instruções,
inconsistência de botões, desalinhamentos e legibilidade. Em ambos os sistemas, a
combinação de desalinhamentos e hierarquia visual insuficiente reforça um padrão
típico de interfaces desenvolvidas sem diretrizes visuais consolidadas, ainda que em
estágios distintos de maturidade.
Achados segundo Nielsen:NoRubricPro, todas as heurísticas foram violadas.
Destacaram-se a falta defeedback, inconsistências linguísticas e ausência de me-
canismos de prevenção de erros. Ferramentas como Heurio e SEER auxiliaram no
mapeamento inicial das ocorrências, que foram validadas manualmente, com precisão
de 81,8% nas sugestões automáticas. NoOsiris, a análise de 38 telas identificou 148
violações confirmadas manualmente. As falhas mais significativas envolveram au-
sência defeedback, inconsistências linguísticas, falta de prevenção de erros e carga
cognitiva elevada decorrente de decisões de layout e conteúdo. A ferramenta SEER
apontou 206 ocorrências, resultando em acurácia final de 71,8%. A convergência en-
tre os dois sistemas indica que problemas de consistência, comunicação e retorno ao
usuário são críticos tanto em aplicações em produção quanto em protótipos de alta
fidelidade.
Achados segundo WCAG:NoRubricPro, a conformidade geral com os critérios
avaliados foi de aproximadamente 30%. Foram identificadas falhas em contraste,
uso deheadings, foco, instruções e rotulagem de links, o que impacta diretamente
a compreensão das ações e a navegação. NoOsiris, a avaliação de 10 critérios
mobile resultou igualmente em 30% de atendimento. As principais falhas incluíram
contraste insuficiente, áreas de toque pequenas, ausência de rótulos em elementos
interativos, links ambíguos e ajuda inconsistente, ainda que aspectos comoreflowe
autenticação tenham sido considerados adequados. A repetição desses padrões em
contextos distintos evidencia a importância de maior atenção a elementos básicos de
legibilidade, foco e clareza das ações oferecidas pelas interfaces.
5.3. IDENTIFICAÇÃO ECLASSIFICAÇÃO DOSPROBLEMAS DEUSABILIDADE
Com base nesses achados, os problemas identificados por C.R.A.P ., Nielsen e
WCAG foram organizados segundo dois critérios complementares:gravidade, fun-
damentada nas diretrizes da ISO 9241-210 para impactos na eficácia, eficiência e
satisfação do usuário (ISO, 2019) e na ISO/IEC 25062 para estimativas de impacto
e esforço de superação (ISO/IEC, 2006), erecorrência, adaptada da escala de se-
veridade de Nielsen (NIELSEN, 1994b), considerando problemas pontuais (até 20%
- baixa), intermediários (20–40% - média) e estruturais (acima de 40% - alta). Essa
abordagem integrada permitiu distinguir falhas isoladas de padrões estruturais, facili-
tando a priorização das recomendações.
NoRubricPro, destacaram-se recorrências elevadas de baixo contraste, desali-
nhamentos, títulos sem marcação semântica e ícones sem rótulo. Já noOsiris, as


ocorrências mais frequentes envolveram ausência de mensagens de erro, inconsis-
tências de capitalização e nomenclatura, legibilidade reduzida, instruções ausentes e
padronização parcial de componentes interativos. Esses padrões são ilustrados nas
Figuras 2 e 3, que apresentam a distribuição das recorrências em cada sistema.
Figura 2 - Avaliação 1: RubricPro
 Figura 3 - Avaliação 2: Osiris
Recorrência dos principais problemas de usabilidade identificados nas duas
avaliações.
Essa categorização integrada evidencia padrões estruturais que comprometem
a clareza visual, a organização espacial e a previsibilidade das interações em am-
bos os sistemas. A aplicação consistente dos mesmos critérios analíticos possibilitou
comparar diretamente a natureza e a frequência dos problemas, estabelecendo um
diagnóstico sólido para orientar recomendações específicas de redesign e servir de
base para a estruturação do guia.
DOCUMENTAÇÃO EREGISTRO DOSACHADOS
Para assegurar rastreabilidade, organização e transparência no processo avalia-
tivo, os achados de ambas as análises foram sistematizados em artefatos complemen-
tares. Para oRubricPro, os resultados foram estruturados em um relatório técnico em
Markdown2e em um quadro interativo no Figma3, contendo anotações diretas sobre
capturas de tela, comparações e agrupamentos por fluxos funcionais.
Ademais, para oOsiris, os achados foram registrados em umboardunificado no
Figma4, reunindo: relatório técnico emMarkdown, protótipo com anotações, exporta-
ções de comentários em planilha, comparativos visuais antes–depois, fluxos revisa-
dos e uma proposta visual refinada, incluindo modo escuro e nova paleta. Comple-
mentarmente, o repositório no GitHub5reúne todos os materiais, incluindo relatório
de problemas por tela e um arquivo de tema CSS com as definições estilísticas pro-
postas.
Esses artefatos reforçam a rastreabilidade das evidências, permitindo acompa-
nhar cada ocorrência desde sua anotação nas telas até sua categorização segundo
C.R.A.P ., Nielsen e WCAG, garantindo consistência entre as duas avaliações e apoi-
ando o processo de síntese comparativa apresentado a seguir.
2Disponível em: <https://github.com/manoelargc/avaliacao-rubric-pro/blob/main/relatorioAnalisePrevia.md>
3Disponível em: <https://www.figma.com/board/h4OqaYbqStyFaNCvzEKT6v/Analise-Rubric-Pro>
4Disponível em: <https://www.figma.com/board/AK2g4XoHmLl0JmWfzFtKSU/Analise-Osiris?node-id=0-1>
5Disponível em: <https://github.com/manoelargc/avaliacao-osiris>


5.4. CONVERGÊNCIAS EDIFERENÇASESSENCIAIS
Os resultados revelaram convergências importantes entre os dois sistemas, so-
bretudo em problemas estruturais de clareza visual, inconsistências terminológicas
e ausência de orientações explícitas ao usuário. Esses problemas apareceram de
maneira consistente independentemente do estágio de maturidade da interface, indi-
cando fragilidades comuns em projetos conduzidos sem diretrizes de design consoli-
dadas.
As diferenças observadas entre os sistemas decorrem principalmente do tipo de
artefato e do contexto de uso. NoRubricPro, um sistema web funcional, os problemas
refletem características de interfaces legadas, como rotulagem incompleta, estrutura
semântica irregular e inconsistências acumuladas ao longo do tempo. NoOsiris, um
protótipomobile-first, as falhas estão associadas à fase inicial de prototipação, inclu-
indo padronização parcial de componentes, capitalização irregular, instruções ausen-
tes e áreas de toque reduzidas, típicas de ambientes móveis.
Houve também diferenças metodológicas relevantes. A avaliação doRubricPro
utilizou oAccessibility Insights for Webpara verificação automatizada de critérios das
WCAG 2.1 e 2.2, o que possibilitou inspeções mais amplas e precisas. NoOsiris,
por se tratar de um protótipo navegável, esse recurso não pôde ser aplicado; assim,
foi adotada uma verificação manual baseada em dez critérios mobile da WCAG 2.2,
selecionados para manter alinhamento conceitual com a primeira avaliação. Essa dis-
tinção explica variações na granularidade da análise e no tipo de problema identificado
em cada sistema.
De forma geral, as convergências revelam padrões estruturais relevantes para
ambos os contextos, enquanto as diferenças reforçam a importância de considerar
dispositivo, estágio de maturidade e ferramentas disponíveis ao avaliar interfaces.
5.5. LIMITAÇÕES, ADAPTAÇÕES ECONCLUSÕES DAAVALIAÇÃOINTEGRADA
A comparação entre os dois sistemas evidenciou não apenas padrões convergen-
tes de problemas de usabilidade, mas também diferenças importantes decorrentes do
tipo de artefato analisado. No caso doRubricPro, a existência de uma aplicação web
funcional permitiu maior apoio de ferramentas automatizadas e inspeções precisas
de elementos interativos reais. Já noOsiris, a ausência de interatividade plena e
a estrutura baseada em protótipo exigiram adaptações metodológicas, sobretudo na
aplicação combinada de WCAG e heurísticas, reforçando a necessidade de triangula-
ção entre métodos e validação humana em cada etapa.
A impossibilidade de executar extensões de navegador sobre protótipos levou à
adoção de uma verificação manual baseada em critérios selecionados da WCAG 2.2
para mobile, o que garantiu continuidade conceitual com a primeira avaliação e possi-
bilitou comparar problemas equivalentes, ainda que com diferentes graus de precisão
operacional. Essa adaptação metodológica foi fundamental para assegurar maior ro-
bustez ao processo avaliativo, preservando o alinhamento entre as duas análises.
Além disso, a natureza estática do protótipo afetou diretamente a acurácia da
ferramenta SEER, resultando em média menor de precisão em comparação à Avalia-
ção 1 (71,8% contra 81,8%). Ainda assim, a média geral das duas avaliações (76,8%)

confirma o potencial do SEER como apoio preliminar à inspeção manual, desde que
utilizado de forma complementar e não substitutiva.
5.6. RECOMENDAÇÕESPRIORITÁRIAS EIMPLICAÇÕES PARA OGUIA
De forma integrada, as recomendações convergem em quatro eixos principais: (i)
melhoria de contraste e legibilidade; (ii) padronização de elementos e capitalização;
(iii) alinhamento e hierarquia visual coerente; e (iv) inclusão de instruções efeed-
backclaros. A síntese desses achados fundamenta diretamente a estrutura do guia
UI4Devs, que organiza essas recomendações em etapas práticas voltadas ao con-
texto de equipes de desenvolvimento sem formação especializada em design.
6. ESTRUTURA EFUNDAMENTAÇÃO DOGUIAUI4DEVS
O guia UI4Devs foi concebido a partir dos achados das Avaliações 1 e 2, que
permitiram identificar padrões recorrentes de problemas de usabilidade em diferentes
contextos de interface. Esses achados foram sintetizados em um conjunto estruturado
de recomendações acionáveis voltadas a equipes de desenvolvimento que, na au-
sência de formação específica em UI/UX, assumem decisões de interface baseadas
sobretudo em experiência prática. O material, formalmente definido comoUI4Devs
(Usability Interface for Developers), destaca tanto seu público-alvo - os desenvolvedo-
res - quanto sua finalidade: oferecer diretrizes de usabilidade acessíveis, aplicáveis e
coerentes com os fluxos reais de trabalho em desenvolvimento de software.
Dessa forma, o guia privilegia clareza, aplicabilidade imediata e independência de
conhecimentos avançados em design, apresentando orientações objetivas que auxi-
liam na melhoria da usabilidade e da acessibilidade ao longo de ciclos iterativos. Sua
estrutura contempla a definição do escopo e do público-alvo, os critérios de organi-
zação do conteúdo e quatro áreas temáticas centrais, cada uma formada por reco-
mendações práticas fundamentadas em heurísticas de Nielsen, nos princípios visuais
C.R.A.P . e nas diretrizes da WCAG.
Essa base teórico-metodológica consolida o UI4Devs como um artefato concei-
tual no âmbito daDesign Science Research, ao reunir modelos, princípios e diretrizes
capazes de orientar a construção de soluções aplicáveis em contextos reais de de-
senvolvimento (GREGOR; HEVNER, 2013; HEVNER et al., 2004). A partir dessa con-
solidação, o guia torna-se o referencial estruturado que fundamenta as decisões de
organização, abrangência e direcionamento das recomendações apresentadas nas
subseções seguintes.
6.1. ESCOPO EPÚBLICOALVO
Em muitos ambientes de desenvolvimento, a responsabilidade por decisões de
interface recai sobre programadores sem conhecimento consolidado em UI/UX, espe-
cialmente em equipes que acumulam funções de implementação e design. Nesses
cenários, referências acessíveis e objetivas são essenciais para orientar melhorias de
clareza visual e usabilidade. O guia responde a essa necessidade ao oferecer um
material conciso e prático, priorizando problemas identificados nas avaliações, como
contraste insuficiente, falta defeedback, desalinhamentos e inconsistências de estilo.


Seu objetivo central é servir como um recurso de consulta rápida que auxilie de-
senvolvedores a identificar e corrigir essas falhas de maneira eficiente, sem exigir co-
nhecimento aprofundado em design. Em vez de discutir aspectos teóricos, o UI4Devs
apresenta recomendações concretas e orientadas à tarefa, aplicáveis em ciclos cur-
tos de desenvolvimento e adequadas para revisões de interface, planejamento visual
e etapas finais antes da publicação.
O público-alvo inclui desenvolvedores, estudantes da área de TI,freelancerse
equipes reduzidas que não contam com designers dedicados. Trata-se também de
um recurso útil em metodologias ágeis, trabalhos acadêmicos, protótipos iniciais e
iniciativas independentes. Ao democratizar boas práticas de UI/UX, o guia contribui
para que equipes técnicas construam sistemas mais consistentes, acessíveis e visu-
almente coerentes mesmo com recursos limitados.
6.2. ESTRUTURA
A organização do UI4Devs reflete diretamente os achados das avaliações. Os
problemas recorrentes identificados foram agrupados em quatro blocos temáticos, ar-
ticulando interseções conceituais entre heurísticas de Nielsen, princípios C.R.A.P . e
diretrizes WCAG. Os blocos são: (i)Legibilidade e Cores, (ii)Navegação e Opera-
bilidade, (iii)Feedbacke Gestão de Errose (iv)Consistência e Padrões Visuais.
Cada bloco reflete padrões críticos observados nas análises e se alinha às dimensões
POUR (Perceptível, Operável, Compreensível e Robusto) da acessibilidade.
A Tabela 2 sintetiza essa relação, evidenciando como cada bloco funciona como
eixo integrado de intervenção ao combinar subsídios provenientes das três aborda-
gens avaliativas. Esse cruzamento fornece um roteiro prático e teoricamente funda-
mentado, permitindo priorizar melhorias com base em evidências e criar uma base
sólida para intervenções sistemáticas.
Tabela 2 - Relação entre grupos temáticos e métodos de avaliação
Grupo Temático Heurísticas de Nielsen Princípios C.R.A.P. Diretriz WCAG
Legibilidade e Cores 1, 2, 3, 6, 8, 9, 10 Contraste e Alinhamento Perceptível
Navegação e Operabilidade 3, 4, 5, 6, 7, 10 Proximidade Operável
Feedbacke Gestão de Erros 1, 3, 5, 9 — Compreensível
Consistência e Padrões Visuais 2, 4, 6 Repetição Robusto
A sequência dos blocos segue uma lógica acumulativa: inicia-se pela clareza
visual (fundamental para percepção), avança-se para navegação e operabilidade,
garante-se a existência defeedbackadequado e, por fim, consolida-se a consistência
estrutural. Essa progressão acompanha o fluxo natural de interação e favorece ciclos
iterativos de aprimoramento.
Para orientar a aplicação prática, o processo é representado por um fluxograma
geral (Figura 4), modelado em BPMN 2.0, que apresenta as quatro etapas e seus
pontos de decisão, tornando o guia utilizável por equipes de desenvolvimento em
ciclos iterativos.
6.3. ETAPAS EATIVIDADES
As etapas e atividades do UI4Devs operacionalizam os blocos temáticos apre-
sentados na subseção anterior, orientando como cada conjunto de recomendações


Figura 4 - Fluxo macro do Guia Prático de UI.
pode ser aplicado no desenvolvimento da interface. Em vez de apresentar apenas
princípios, esta subseção detalha ações práticas que o desenvolvedor deve executar
para incorporar gradualmente as melhorias propostas.
Legibilidade e Cores:reúne diretrizes voltadas à construção de interfaces per-
ceptíveis e visualmente estáveis. A etapa abrange definição de paletas acessíveis,
organização tipográfica e configuração visual coerente de componentes, integrando
recomendações da WCAG, dos princípios C.R.A.P . e de heurísticas sobre visibilidade
e consistência.
As atividades compreendem:
1.Paleta de cores acessível: definição de uma cor primária e geração de cores
secundárias e semânticas (sucesso, alerta e erro), assegurando relações de con-
traste compatíveis com WCAG AA;
2.Tipografia e hierarquia visual: seleção de uma família tipográfica e construção
de uma hierarquia (títulos, subtítulos, corpo e legendas) com parâmetros de ta-
manho, peso e espaçamento que sustentem diferenciação clara entre níveis de
informação;
3.Configuração de componentes: especificação de raio de borda e padroniza-
ção de variantes de botões (preenchido, contornado, ghost, desabilitado), pre-
servando uniformidade visual e adequação para interação em interfaces móveis.
Navegação e Operabilidade:trata dos elementos que estruturam o desloca-
mento do usuário e a compreensão do fluxo. A etapa reúne normas de organização
espacial, sinalização de localização e mecanismos que reduzem carga de memori-
zação, alinhando-se às heurísticas de controle do usuário, consistência e reconheci-
mento, ao princípio de proximidade do C.R.A.P . e às diretrizes de operabilidade da
WCAG.
As atividades incluem:
1.Margens, espaçamento e responsividade: definição de grades adaptadas a
diferentes resoluções (desktopemobile);

2.Indicadores de localização e progresso: especificação de padrões debread-
crumbe elementos de progresso para reforçar orientação e acompanhamento de
etapas;
3.Dimensão de ícones e áreas de toque: parametrização de ícones com 24×24px
e alvos de toque com 44×44px, garantindo precisão e acessibilidade principal-
mente em ambientes móveis;
4.Desfazer, confirmar e ações seguras: estabelecimento de critérios para ações
críticas, incluindo diálogos de confirmação e notificações temporárias com opção
de reversão.
Feedback e Gestão de Erros:consolida práticas relacionadas à comunicação
entre sistema e usuário, com ênfase na previsibilidade de estados, prevenção de erros
e clareza nas mensagens de recuperação. A etapa integra heurísticas de visibilidade
do status, prevenção e recuperação de erros, além do princípio “Compreensível” da
WCAG.
As atividades são estruturadas em:
1.Feedbackvisual após ações: especificação de elementos de carregamento e
notificações, com diretrizes sobre posicionamento, duração e critérios de aciona-
mento;
2.Confirmações de ações críticas: definição de padrões para validação de ações
irreversíveis, com uso de modais e confirmações em múltiplas etapas quando
necessário;
3.Validação progressiva: determinação de padrões de validação durante o preen-
chimento de campos, com uso de cores e textos auxiliares para indicar sucesso
ou erro;
4.Mensagens de erro claras: elaboração de critérios de redação voltados a des-
crever a causa provável do erro e os passos para sua correção, utilizando lingua-
gem objetiva;
5.Ajuda contextual: organização de camadas de suporte, comotooltips, textos
explicativos e guias rápidos, posicionados para complementar a interação sem
sobrecarga cognitiva.
Consistência e Padrões Visuais:reúne orientações para construção de interfa-
ces previsíveis e facilmente escaláveis. A etapa aborda padronização visual, uniformi-
dade linguística e organização modular dos elementos, baseando-se em heurísticas
de consistência, no princípio de repetição do C.R.A.P . e nas recomendações de ro-
bustez da WCAG.
As atividades contemplam:
1.Sistema padronizado de espaçamento: definição de escalas baseadas em
múltiplos de 8px para margens,paddingse espaçamentos internos, criando ritmo
visual uniforme;
2.Padronização de ícones: adoção de uma biblioteca única e de um estilo visual
coerente, preservando significado e peso visual consistentes;

3.Linguagem e nomenclatura uniformes: estabelecimento de regras de capita-
lização, tom de voz e terminologia, aplicadas de maneira uniforme em toda a
interface;
4.Biblioteca de componentes: definição de diretrizes para criação ou combina-
ção deframeworkse componentes customizados, incluindo documentação de
propriedades, variantes e requisitos de acessibilidade.
O guia combina explicações curtas e exemplos visuais, permitindo que desen-
volvedores identifiquem e corrijam problemas sem depender de formação formal em
design. Seu fluxo favorece melhorias incrementais integradas a revisões de código,
sprints ágeis ou rotinas de avaliação.
Em vez de substituir processos de design centrados no usuário, o UI4Devs atua
como um atalho prático para tratar falhas comuns. Sua natureza incremental reduz
retrabalho, acelera iterações e aumenta a confiabilidade das interfaces produzidas.
Os próximos passos incluem validar o guia junto a equipes técnicas, coletarfeedback
sobre clareza e aplicabilidade e aprimorá-lo em ciclos contínuos. Para ampliar seu
alcance e facilitar sua adoção, o guia foi ainda convertido em uma aplicação web.
Essa implementação dá origem ao MVP apresentado na próxima seção.
7. MVP UI4DEVS
O Produto Mínimo Viável (MVP) do UI4Devs6representa a materialização prática
das diretrizes consolidadas no guia, configurando o artefato instanciado no contexto
daDesign Science Research. A escolha por um MVP alinha-se à definição de Ca-
roli (2018), para quem esse tipo de entrega corresponde à versão mais simples de
um produto capaz de validar hipóteses essenciais, permitindo aprender rapidamente
sobre seu funcionamento e evitar o desperdício de tempo, esforço e recursos no de-
senvolvimento de soluções que não atendam às necessidades reais do usuário.
Nesse sentido, transformar recomendações teóricas em uma aplicação web na-
vegável e orientada à tomada de decisão permite verificar, de forma direta, a utilidade
prática das diretrizes propostas. O MVP concretiza o conteúdo conceitual apresen-
tado na Seção 6, oferecendo um ambiente controlado para testar clareza, aplicabili-
dade e fluidez das etapas do guia.
Nesta seção, descrevem-se o desenvolvimento do MVP , sua motivação estraté-
gica, requisitos, arquitetura, tecnologias, identidade visual e funcionalidades imple-
mentadas. O artefato foi projetado para avaliar, junto ao público-alvo, a capacidade
do guia de apoiar decisões de interface e orientar processos de melhoria em equipes
predominantemente técnicas.
7.1. LEANCANVAS
Antes da implementação, foi necessário organizar de forma objetiva quais pro-
blemas o MVP deveria validar e qual valor mínimo deveria ser entregue. Conforme
discute Caroli (2018), a reflexão sobre foco, hipóteses e valor essencial costuma ser
estruturada no canvas MVP(etapa central do Lean Inception), mas sua lógica de va-
lidação incremental também se alinha a modelos enxutos como oLean Canvas. Por
6Disponível em: <https://ui4devs.vercel.app>


esse motivo, adotou-se oLean Canvascomo instrumento inicial de planejamento, já
que ele sintetiza, em uma única etapa e estrutura, o problema, a proposta de valor, os
segmentos de usuários, os canais e as métricas essenciais.
Nesse contexto, o desenvolvimento do UI4Devs foi conduzido com base noLean
Canvas, modelo visual proposto por Maurya (2012) para organizar soluções digitais
em estágio inicial, conforme mostra a Figura 5. A aplicação desse modelo permitiu
alinhar as decisões fundamentais às necessidades do público-alvo, evidenciando três
problemas recorrentes entre desenvolvedores: a dificuldade na tomada de decisões
de interface, a escassez de materiais objetivos voltados ao contexto técnico e a fre-
quência de erros básicos de usabilidade.
Figura 5 - Lean Canvas
A partir desse mapeamento e considerando o escopo do guia, foram refinados os
segmentos de clientes e os requisitos funcionais prioritários, apresentados na próxima
subseção. OLean Canvastambém orientou a definição dos canais de divulgação,
como web e redes sociais, e das métricas utilizadas no survey, incluindo conclusão
dos módulos, tempo médio de uso e clareza percebida.
Por fim, seus componentes oferecem subsídios para a criação de uma futuralan-
ding pagefocada em conversão, ao explicitar de forma clara o problema, a solução e
a proposta de valor. Essa base estratégica também favorece a evolução do UI4Devs
como produto digital, conforme discutido por Drongelen, Dennis e Garabedian (2017).
7.2. REQUISITOSFUNCIONAIS
Os requisitos funcionais da aplicação foram definidos com base na análise do
fluxo proposto pelo guia, considerando também os componentes estratégicos mape-
ados noLean Canvas, como os problemas priorizados, segmentos de clientes e pro-
posta de valor. O objetivo foi transformar as diretrizes em funcionalidades essenciais
dentro de um ambiente interativo. Cada requisito descreve uma capacidade neces-
sária para que o usuário consiga percorrer os módulos, registrar escolhas, visualizar
resultados e compreender as orientações aplicadas ao seu projeto. A Tabela 3 apre-
senta os requisitos organizados de forma clara e sistemática.
Esses requisitos refletem o núcleo funcional do artefato instanciado: iniciar uma


avaliação, conduzir o usuário por etapas sequenciais, permitir interações configurá-
veis (como seleção de cores e parâmetros tipográficos), registrar o progresso e apre-
sentar um resumo final consolidado. O conjunto foi planejado para manter o MVP leve,
objetivo e alinhado ao propósito de validação, garantindo que o foco permanecesse
na experiência do usuário e na aplicabilidade das diretrizes do guia em um cenário
real de uso.
Tabela 3 - Requisitos Funcionais do MVP UI4Devs
ID Descrição
RF1 Cadastro do nome do sistema ou projeto para iniciar a avaliação.
RF2 Navegação sequencial entre os quatro módulos com barra de progresso.
RF3 Execução de etapas interativas (seleções, geração de paletas, pré-visualizações).
RF4 Salvamento automático do progresso do usuário dentro de cada módulo.
RF5 Exibição de resumo final contendo todas as decisões registradas durante a avaliação.
RF6 Interface responsiva funcionando adequadamente em desktop e dispositivos móveis.
7.3. REQUISITOSNÃOFUNCIONAIS
Os requisitos não funcionais complementam a estrutura do MVP ao definir crité-
rios de qualidade essenciais para que o artefato instanciado ofereça uma experiência
consistente, acessível e tecnicamente adequada. Parte desses requisitos também se
alinha aos elementos estratégicos identificados noLean Canvas, como os canais de
acesso e as métricas de sucesso, que demandam uma interface funcional, respon-
siva e clara. Como o objetivo do MVP é permitir a validação prática das diretrizes do
UI4Devs, esses requisitos foram estabelecidos para garantir que o produto funcione
de maneira fluida e confiável, independentemente do ambiente de uso.
A Tabela 4 apresenta os requisitos definidos, que abrangem usabilidade, acessibi-
lidade, desempenho, manutenibilidade e escalabilidade visual. Entre eles, incluem-se
a necessidade de contraste mínimo conforme WCAG AA, responsividade, microinte-
rações claras, carregamento leve e uso de componentes reutilizáveis. Esses aspectos
asseguram que o MVP mantenha um padrão mínimo de qualidade e reflita, em sua
própria interface, as práticas recomendadas pelo guia.
Tabela 4 - Requisitos Não Funcionais do MVP UI4Devs
ID Descrição
RNF1 Usabilidade: interface clara, objetiva e com microinterações que auxiliem o uso.
RNF2 Acessibilidade: contraste mínimo AA e áreas de toque com dimensão adequada.
RNF3 Desempenho: carregamento leve e navegação fluida entre módulos e etapas.
RNF4 Manutenibilidade: código modular e baseado em componentes reutilizáveis.
RNF5 Escalabilidade visual: utilização consistente de cores, espaçamentos e tipografia.
7.4. ARQUITETURA EMODELO DEDADOS
A arquitetura do UI4Devs foi concebida para permitir evolução gradual do sis-
tema e manter alinhamento com o propósito do MVP enquanto artefato instanciado
no contexto da DSR. Para a etapa de validação conduzida neste estudo, a aplicação
foi disponibilizada aos participantes funcionou exclusivamente nofrontend, uma vez
que obackendencontra-se em desenvolvimento no escopo deste trabalho.
Para assegurar o funcionamento completo do fluxo de avaliação, ofrontenduti-
lizou dadosmockadosarmazenados nolocalStorage, permitindo simular o compor-


tamento esperado do sistema sem comprometer a experiência do usuário. O geren-
ciamento do estado global foi centralizado noEvaluationContext, implementado com
React Context API, garantindo consistência entre etapas e permitindo substituição
futura para obackenddefinitivo.
Estruturalmente, ofrontendfoi organizado em Next.js com App Router, utilizando
rotas dinâmicas e módulos independentes. A separação de responsabilidades foi
distribuída entre diretórios comoservices/(comunicação com a API futura),types/
(tipagens TypeScript),hooks/(lógica reutilizável),contexts/(estado global) elib/
(utilidades). Essa estrutura modular facilita manutenção, testes e expansão, permi-
tindo incorporar autenticação, sincronização e múltiplas avaliações por usuário em
versões subsequentes.
Apesar de o MVP utilizado nosurveyoperar somente nofrontend, a arquitetura
geral foi planejada para garantir continuidade, escalabilidade e aderência às neces-
sidades futuras do projeto, preservando o alinhamento entre o artefato conceitual (o
guia) e sua implementação prática.
7.5. TECNOLOGIASUTILIZADAS
Quanto às tecnologias utilizadas, a ferramenta foi desenvolvida com Next.js 14,
adotado pelo suporte a rotas dinâmicas, organização modular e integração direta com
a Vercel, permitindodeploycontínuo durante o ciclo de testes. A interface foi constru-
ída com Tailwind CSS, facilitando a criação de layouts responsivos e a aplicação dos
tokensde cor e tipografia definidos no guia. Todo o código foi escrito em TypeScript
para aumentar segurança e reduzir erros, com versionamento realizado via GitHub.
Como obackendainda estava em desenvolvimento, algumas limitações envolve-
ram o uso dolocalStorageem ambiente de renderização no servidor e o ajuste entre
dadosmockadose a futura API. Ainda assim, o conjunto de tecnologias adotado ga-
rantiu um MVP leve, consistente e adequado à etapa de validação.
7.6. IDENTIDADEVISUALUI4DEVS
A identidade visual do UI4Devs, apresentada na Figura 6, elaborada pela autora,
foi definida para refletir clareza, simplicidade e alinhamento ao universo dos desenvol-
vedores. O símbolo combina três elementos: o contorno arredondado representando
a interface gráfica, as marcas “<>” que remetem ao código, e o cursor de mouse,
fazendo uma referência direta ao dispositivo inovador introduzido por Douglas Engel-
bart na década de 1960, que marcou a transição para interações mais intuitivas na
moderna GUI. Essa combinação sintetiza tanto o ato de desenvolver quanto a experi-
ência de interagir com interfaces digitais.
A tipografia utiliza a família Ubuntu, escolhida pela legibilidade, formas suaves e
associação visual a ambientes de programação. O uso de letras minúsculas reforça a
proposta de aproximação com o público-alvo, mantendo um caráter direto e funcional.
A paleta cromática adota o verde como cor primária, apoiada em referências da
psicologia das cores ligadas à tecnologia e em conexões históricas com monitores
de console. Tons complementares de preto, cinza e branco garantem contraste ade-
quado e compatibilidade com temas claro e escuro.


Figura 6 - Identidade Visual UI4Devs
Os componentes seguem o mesmo racional visual: cantos levemente arredon-
dados, ícones padronizados e microinterações discretas para estados e progressões.
Assim, a identidade visual reforça no próprio MVP os princípios de consistência e
clareza promovidos pelo guia.
7.7. FUNCIONALIDADES ETELAS DOMVP
O MVP UI4Devs foi estruturado em quatro módulos correspondentes às etapas
do guia, cada um composto por tarefas guiadas e elementos interativos. O fluxo
inicia na tela de criação do projeto (Figura 7), em que o usuário informa o nome do
sistema a ser avaliado. Em seguida, é direcionado ao painel principal, que apresenta
o progresso geral e permite iniciar cada módulo.
Figura 7 - Tela inicial do UI4Devs, exibida em modo claro e modo escuro.
A estrutura completa das telas está organizada na Figura 8. As setas contínuas
indicam navegação hierárquica, enquanto a seta tracejada representa a ação global
de reiniciar a avaliação. A legenda diferencia os tipos de elementos exibidos nas telas,
facilitando a leitura e evidenciando o papel de cada componente no fluxo.


Figura 8 - Organização e hierarquia das telas do MVP UI4Devs
No Módulo 1 (Figura 9), o usuário define a paleta de cores, seleciona a tipogra-
fia e configura componentes. Ao final, uma tela de síntese apresenta as conquistas
adquiridas, um resumo das escolhas feitas no módulo e opções de exportaçãoMark-
down(e também .css, dependendo no módulo). As telas incluem microinterações,
estados de carregamento, barras de progresso e ícones informativos que reforçam a
orientação em cada etapa.
Figura 9 - Algumas telas do módulo de Legibilidade e Cores.
Todos os módulos seguem a mesma lógica: atividades objetivas combinando eta-
pas interativas e informativas, validações visuais e uma tela de síntese consolidada.
Esse formato foi delineado a partir da proposta de valor definida noLean Canvas, que
posiciona o UI4Devs como um guia acessível e prático para apoiar decisões de inter-


face por parte de desenvolvedores. Assim, o MVP demonstrou, na prática, a aplicação
das recomendações do guia e apoiou a coleta de dados para validação.
7.8. SÍNTESE
O MVP UI4Devs materializou, em uma aplicação web, as diretrizes estruturadas
no guia, organizando-as em módulos guiados que possibilitam escolhas de interface
aplicadas de forma prática. O sistema incorporou elementos essenciais para essa
experiência, como fluxos sequenciais, microinterações, barras de progresso, expor-
tações e resumos finais, garantindo coerência entre teoria e aplicação. A combina-
ção de Next.js, Tailwind CSS e TypeScript assegurou responsividade e consistência
visual, enquanto a identidade visual reforçou simbolicamente a relação entre desen-
volvimento e interação.
Embora obackendestivesse em fase de modelagem, o uso de dadosmockados
vialocalStoragepermitiu que o MVP funcionasse integralmente, garantindo a execu-
ção do fluxo completo de avaliação. Essa configuração foi suficiente para a etapa de
validação, permitindo coletar percepções reais sobre utilidade, clareza e aplicabilidade
das recomendações. Assim, o MVP cumpriu seu papel como artefato instanciado na
DSR, servindo simultaneamente como demonstração funcional das diretrizes e como
base empírica para evolução futura do sistema.
8. VALIDAÇÃO DOGUIA
A validação do Guia Prático de UI foi conduzida por meio de um protocolo desur-
veyestruturado em dois formulários complementares, pré-uso e pós-uso, projetados
para capturar tanto o perfil e as expectativas dos participantes quanto suas percep-
ções após a utilização da ferramenta. O objetivo central dessa etapa foi verificar, junto
ao público-alvo, a clareza, utilidade e aplicabilidade prática do material desenvolvido,
assegurando que o guia atendesse efetivamente às necessidades de estudantes e
profissionais envolvidos no desenvolvimento de interfaces.
8.1. PROTOCOLO DOSURVEY
Osurveyfoi estruturado com base em um protocolo que definiu claramente o
objetivo da pesquisa, suas perguntas norteadoras, o público-alvo e o plano de amos-
tragem utilizado para a coleta dos dados.
Objetivo da Pesquisa.O objetivo central dosurveyfoi validar o Guia Prático
de UI junto ao público-alvo, examinando sua clareza, utilidade e aplicabilidade em
diferentes contextos de uso. Buscou-se compreender como o guia se comporta na
prática e em que medida apoia estudantes e profissionais no processo de melhoria
de interfaces.
Perguntas de Pesquisa.A condução dosurveyfoi orientada pelas seguintes
questões:
• O guia é claro e fácil de seguir para usuários com diferentes níveis de experiên-
cia?
• Os módulos e etapas são úteis e aplicáveis na prática de criação ou melhoria de
interfaces?

• Em que tipos de projeto o guia tende a ser utilizado e qual a percepção dos
participantes sobre sua eficácia?
• Os usuários recomendariam e reutilizariam o guia em outros contextos?
Público-Alvo.Foram considerados como público-alvo estudantes de Ciência da
Computação e Engenharia de Software da UNIPAMPA, participantes do Programa de
Pós-Graduação em Engenharia de Software (PPGES) e profissionais com experiência
em desenvolvimento ou design de interfaces. A definição buscou contemplar perfis
que, na prática, poderiam se beneficiar diretamente do uso do guia.
Plano de Amostragem.O survey utilizou uma amostragem não probabilística
por conveniência, baseada nos canais de acesso disponíveis à autora. O formulário
de pré-uso foi divulgado por e-mail institucional para as listas dos cursos de Ciência
da Computação e Engenharia de Software da UNIPAMPA, em grupos de WhatsApp
associados a esses cursos e no grupo do PPGES. A chamada também foi publicada
no LinkedIn da autora e enviada diretamente a profissionais e colegas da área. Após
o preenchimento do pré-uso, os participantes eram automaticamente direcionados ao
formulário de pós-uso, assegurando a continuidade do protocolo de validação.
O processo foi dividido em duas etapas complementares: o formulário de pré-uso,
destinado à caracterização dos respondentes e ao levantamento de suas expectati-
vas, e o formulário de pós-uso, aplicado após a navegação no guia. Essa divisão
permitiu medir tanto o perfil e as expectativas iniciais quanto a percepção após a ex-
periência prática com o material.
8.2. EXECUÇÃO
A validação foi conduzida em duas etapas sequenciais: pré-uso e pós-uso, ao
longo de um período total de 10 dias (de 17/11/2025 até 27/11/2025) em que o guia
permaneceu disponível para avaliação. No total, 77 participantes responderam ao
formulário inicial e 44 concluíram também o formulário de pós-uso. Apenas estes
últimos foram considerados na análise final. O último bloco do pré-uso continha o link
direto para a ferramenta e para o questionário pós-uso, assegurando a continuidade
do protocolo e permitindo mapear apenas os participantes que efetivamente utilizaram
o guia.
O formulário de pré-uso foi estruturado em três blocos. O primeiro abrangeu o
Termo de Consentimento Livre e Esclarecido (TCLE) e o Perfil do Participante, in-
cluindo faixa etária, função principal, tempo de experiência na área e tipo de projeto
em que atua com maior frequência. O segundo bloco tratou da experiência e conhe-
cimento em UI, reunindo questões sobre nível de domínio em design de interfaces,
etapa do desenvolvimento em que o participante possui mais facilidade e frequência
com que aplica boas práticas de interface. O terceiro bloco abordou as expectativas
sobre o guia, por meio de uma escala de 1 a 5 sobre o quão útil o material poderia
ser para sua prática.
O questionário do formulário de pós-uso, acessado após a navegação no guia,
também foi dividido em três blocos. O primeiro registrou o contexto de aplicação, in-
cluindo horário de início e fim do teste, tipo de projeto em que o guia foi utilizado,
tempo dedicado e módulos concluídos. O segundo bloco avaliou a percepção de

utilidade e clareza, com itens em escala de 1 a 5 sobre facilidade de seguir o guia, ob-
jetividade das instruções, apoio na identificação de problemas não percebidos, contri-
buição para o raciocínio de design e utilidade para projetos futuros, além de perguntas
sobre o módulo mais útil, o mais cansativo e a intenção de reutilizar ou recomendar
o guia. O terceiro bloco coletou comentários abertos, permitindo que os participantes
registrassem críticas, percepções gerais e sugestões de melhoria.
A divulgação dos formulários ocorreu por e-mail institucional, grupos de What-
sApp dos cursos de Ciência da Computação e Engenharia de Software da UNIPAMPA,
no grupo do PPGES e em postagem no LinkedIn da autora, além de convites diretos.
Essa estratégia assegurou amplo alcance dentro do público inicialmente previsto e
também possibilitou a participação de perfis externos, ampliando a diversidade de
perspectivas contempladas na validação.
8.3. ANÁLISE DOSRESULTADOS
A análise dos dados coletados no pré-uso e pós-uso permitiu compreender o
perfil dos participantes, suas expectativas iniciais, a experiência prática com o guia
e a percepção global sobre sua clareza, utilidade e aplicabilidade. As evidências
foram organizadas a partir de dados quantitativos e qualitativos, apoiando a avaliação
integrada da ferramenta.
Perfil dos Respondentes.A etapa de pré-uso contou com 77 respostas, pos-
sibilitando caracterizar o público participante. A Figura 10 sintetiza a distribuição da
função principal, evidenciando a predominância de desenvolvedores (75%), seguidos
por designers de interface/UX, estudantes e profissionais de QA.
Desenvolvedor
Estudante
Design de Interface / UX
Outros
33 (75.0%)5 (11.4%)3 (6.8%)3 (6.8%)
Figura 10 - Função principal declarada pelos participantes.
Quanto ao tempo de experiência profissional (Figura 11), a maioria declarou atuar
entre 1 e 3 anos (43,2%), reforçando o perfil de profissionais em início de carreira.
O conhecimento prévio em design de interfaces (Figura 12) concentrou-se nos ní-
veis intermediários baixos: 63,6% atribuíram-se ao nível 3 e 25% ao nível 2, enquanto
apenas 11,3% declararam domínio elevado (níveis 4 ou 5).
Além disso, 43,2% afirmaram depender frequentemente de referências prontas
na criação de interfaces e 29,5% relataram preferência por trabalhar com designs


0 5 10 15 20Menos de 1 ano1 a 3 anos4 a 6 anos7 a 10 anosMais de 10 anos
7(15.91%)19(43.18%)12(27.27%)2(4.55%)4(9.09%)
Figura 11 - Tempo de experiência na área de atuação.
0 5 10 15 20 25 30Nível 1Nível 2Nível 3Nível 4Nível 5
0(0%)11(25%)28(63.64%)4(9.09%)1(2.27%)
Figura 12 - Nível de conhecimento autodeclarado em design de interfaces.
previamente definidos, indicando limitações de autonomia no processo de design.
Ainda assim, as expectativas sobre o guia foram altas: 75% atribuíram nota máxima
ao seu potencial de utilidade. O formulário de pós-uso contou com 44 respostas. Em
relação ao contexto de uso, 34,1% aplicaram o guia em projetos pessoais, 15,9% em
projetos acadêmicos, 11,4% em projetos profissionais e 38,6% apenas exploraram o
conteúdo sem uso aplicado.
Complementarmente, por meio da ferramenta Analytics da Vercel e da análise dos
domínios de e-mail institucional dos respondentes, verificou-se que o guia alcançou
pelo menos um representante de cada um dos 10 estados brasileiros (RS, SC, GO,
DF , AM, CE, SP , MG, PR e RJ) e também de 3 países (Brasil, Argentina e Áustria),
conforme ilustrado na Figura 13. O Analytics também indicou que 73% dos testes
foram realizados em dispositivos desktop, enquanto 27% ocorreram em dispositivos
móveis, sugerindo que a maioria dos usuários acessou o guia em ambientes associ-
ados a atividades de desenvolvimento.
Resultados Quantitativos do Pós-Uso.O tempo de utilização confirmou o ca-
ráter leve e objetivo do guia: 65,9% concluíram as etapas em menos de 15 minutos
e 31,8% entre 15 e 30 minutos. As taxas de conclusão por módulo foram elevadas:
100% (Legibilidade e Cores), 97,7% (Navegação e Operabilidade) e 93,2% nos de-
mais. A Figura 14 sintetiza as percepções gerais de clareza, utilidade e facilidade
de uso do guia, com base nas respostas às cinco questões centrais do questioná-
rio pós-uso. As questões (Q1–Q5) foram avaliadas em uma escala do tipo Likert de
5 pontos, conforme proposta originalmente por Likert (1932) e aplicada segundo as
recomendações metodológicas discutidas por Joshi et al. (2015), variando de “nada”
(1) a “totalmente” (5), o que permitiu mensurar de forma estruturada o grau de cla-
reza, utilidade e impacto do guia na prática dos participantes. A Tabela 5 sumariza as
questões aplicadas no questionário pós-uso do guia UI4Devs.
Os resultados indicam forte concentração nos níveis mais altos da escala. Em
Q1, 90,9% atribuíram nota 5 para a facilidade de seguir o guia. Em Q2, 100% dos


Figura 13 - Distribuição geográfica dos respondentes.
Código Descrição da Questão
Q1 O quanto o guia foi fácil de seguir.
Q2 O quanto as instruções foram claras e objetivas.
Q3 O quanto o guia ajudou a identificar problemas de design não percebidos anteriormente.
Q4 O quanto o guia contribuiu para melhorar o raciocínio de design do participante.
Q5 O quanto um guia interativo como este seria útil em futuros projetos.
Tabela 5 - Questões do questionário pós-uso do guia UI4Devs.
0 20 40 60 80 100Q1
Q2
Q3
Q4
Q590.9%
86.4%
47.7%
63.6%
88.6%9.1%
13.6%
34.1%
29.5%
6.8%18.2%
6.8%
4.5%
Nada Pouco Neutro Muito Totalmente
Figura 14 - Síntese das respostas de clareza, utilidade e facilidade de uso (Q1–Q5).
respondentes avaliaram as instruções como claras e objetivas (notas 4 ou 5). Em Q3,
84,1% relataram que o guia os ajudou a identificar problemas de design antes não
percebidos. Tendências semelhantes emergiram em Q4 e Q5, reforçando o impacto
positivo do material tanto no desenvolvimento do olhar crítico quanto na expectativa
de uso futuro.
A análise complementar, apresentada na Figura 15, compara o benefício perce-
bido e o nível de cansaço em cada módulo. Os resultados mostram predominância de
avaliações positivas em todos os blocos, com destaque para Consistência e Padrões
Visuais (36,4% como módulo mais útil) e Legibilidade e Cores (34,1%). Além disso,


47,7% dos respondentes relataram que nenhum módulo foi cansativo, sugerindo boa
distribuição do conteúdo e adequado equilíbrio entre etapas informativas e interativas.
0 20 40 60 80 100Mais benefícios
Mais cansativo 46.7%37.8%
26.6%20%
8.9%8.9%
15.6%33.3%
2.2%
Legibilidade e cores Navegação e operabilidade Feedback e erros
Consistência e Padrões Nenhum
Figura 15 - Percepção de benefício e cansaço por módulo.
A intenção de reutilização foi expressiva: 86,4% afirmaram que utilizariam o guia
novamente e 93,2% recomendariam o material a outros profissionais.
Análise Qualitativa:A análise qualitativa das respostas abertas foi realizada a
partir da questão final do formulário pós-uso, dedicada ao bloco deFeedbacke Su-
gestões - Comentário Final. O processo adotou uma codificação temática sistemática,
permitindo identificar padrões recorrentes, percepções compartilhadas e sugestões
específicas sobre o uso do guia. Ao todo, 25 dos 44 participantes contribuíram com
comentários textuais, resultando em 66 trechos codificados, conforme sintetizado na
Tabela 6. As respostas variaram entre observações breves e relatos mais elaborados,
refletindo diferentes níveis de engajamento e detalhamento nas contribuições.
Tabela 6 - Estatísticas Relacionadas aos Códigos e Citações
Métrica Valor
Número total de trechos codificados 66
Número de citações positivas 52
Número de citações negativas 5
Número de sugestões de melhoria 10
Número de códigos identificados 9
Ao todo, foram identificados nove códigos, distribuídos em três categorias princi-
pais:FeedbackPositivo,FeedbackNegativo e Sugestões de Melhorias. A árvore de
códigos gerada pela ferramenta de análise qualitativaQAnubis(Figura 16) sintetiza
essa organização. Os resultados mostram predominância de percepções positivas,
com 52 trechos associados a elogios ou avaliações favoráveis, 5 trechos relacionados
a aspectos negativos e 10 sugestões adicionais que ampliaram a compreensão geral
sobre o uso e o potencial de evolução do guia.
Entre os códigos positivos, destacam-se principalmente Utilidade Prática (21 ocor-
rências) e Aprendizado e Caráter Didático (14 ocorrências). Esses códigos refletem
que o guia foi percebido como um recurso efetivo para apoiar decisões de design, faci-
litar a compreensão de padrões e orientar usuários com pouca experiência prévia em
UI. Comentários sobre Clareza e Facilidade de Uso (10 ocorrências) reforçam a boa
organização dos módulos, a objetividade das instruções e a facilidade de navegação.
Também foram recorrentes elogios à Interface Agradável e Organização (7 ocorrên-
cias), indicando que a forma como o conteúdo é apresentado contribui positivamente
para a experiência geral de uso.
No conjunto de códigos negativos, apareceram menções pontuais aBugsou
Problemas Técnicos (2 ocorrências) e a Problemas dePreviewou Interatividade (2
ocorrências), além de um único comentário relacionado a Excesso de Informação.


Figura 16 - Árvore dos códigos identificados e suas categorias
Embora pouco frequentes, esses registros apontam pontos de aprimoramento espe-
cíficos, principalmente relacionados à estabilidade da ferramenta e à clareza visual
das prévias exibidas durante o uso.
As sugestões de melhoria também forneceram contribuições relevantes, princi-
palmente em duas frentes: expansão de conteúdo (6 ocorrências), como inclusão
de novos módulos e aprofundamentos, e melhorias de abordagem (3 ocorrências),
sobretudo relacionadas à interatividade, dinamicidade e maior detalhamento pedagó-
gico. Esses apontamentos reforçam o interesse dos participantes em versões mais
completas e robustas do guia, sem comprometer a leveza e a clareza que caracteri-
zaram a experiência atual.
Por fim, a nuvem de palavras gerada a partir dos códigos, apresentada na Fi-
gura 17, evidencia visualmente os códigos mais mencionados, com destaque para
expressões como “utilidade prática”, “aprendizado”, “clareza” e “interface organizada”.
Figura 17 - Nuvem de palavras de códigos
8.4. DISCUSSÃO DOSRESULTADOS
Os resultados obtidos permitem afirmar que o Guia Prático de UI atendeu ao obje-
tivo de oferecer um material claro, acessível e aplicável para usuários com diferentes


níveis de familiaridade com design de interfaces. A caracterização inicial do público
indica um perfil majoritariamente jovem, composto sobretudo por desenvolvedores
com pouca ou moderada experiência em UI, muitos dos quais relataram depender de
referências prontas ou de terceiros para tomar decisões visuais. Esse cenário reforça
a relevância do guia como ferramenta de apoio para equipes técnicas que enfrentam
insegurança ou lacunas conceituais ao trabalhar com aspectos visuais de interfaces.
As percepções pós-uso confirmam essa necessidade e revelam que o guia de-
manda baixo esforço cognitivo. A maioria dos participantes concluiu o material em
menos de 15 minutos, o que evidencia sua leveza e sua adequação ao propósito de
consulta rápida, especialmente em ambientes de desenvolvimento que exigem solu-
ções práticas e objetivas. A elevada taxa de conclusão dos módulos e a forte con-
centração de notas máximas em clareza e facilidade de uso indicam que a estrutura
modular, oschecklistse a linguagem direta contribuíram para uma experiência fluida e
sem barreiras de compreensão, coerente com o propósito do guia de funcionar como
recurso prático e de consulta rápida.
Além da boa recepção, observou-se impacto efetivo na forma como os participan-
tes analisam interfaces. Uma parcela expressiva relatou ter identificado problemas de
UI que antes não percebiam, especialmente em dimensões como legibilidade, consis-
tência e padronização visual. Esse resultado sugere que o guia não apenas entrega
instruções, mas também amplia o repertório analítico dos usuários, fortalecendo o
pensamento crítico em design. Essa interpretação é reforçada pela convergência
entre os dados quantitativos (altas notas em Q3 e Q4) e qualitativos (códigos como
“Aprendizado” e “Utilidade Prática”).
Outro ponto relevante diz respeito ao alcance geográfico diversificado da valida-
ção. A participação de respondentes distribuídos por diferentes estados brasileiros
e também por outros países mostra que o material despertou interesse para além
do círculo institucional imediato e do público mais próximo da autora, ampliando a
representatividade dos resultados. O predomínio de acessos viadesktoptambém
se mostrou coerente com o perfil dos participantes e com a natureza da atividade,
geralmente realizada em contextos de desenvolvimento ou estudo.
A análise qualitativa complementa e reforça esses achados. Os comentários es-
pontâneos evidenciaram ampla satisfação com a clareza, organização e utilidade prá-
tica do guia, além de destacarem seu caráter didático. Muitos participantes relataram
que o material favoreceu o aprendizado e facilitou a compreensão dos padrões de
interface. Um dos depoimentos ilustra bem esse aspecto ao afirmar que o guia é
“simples, didático e completamente necessário [...] ensina métodos pelos quais de-
terminadas pessoas passariam sem notar” (S06), evidenciando seu valor pedagógico
para usuários com pouca experiência prévia em UI. Também houve menções ao apoio
na tomada de decisão e na organização das escolhas de design, como no comentá-
rio de que “os exemplos apresentados [...] oferecem uma boa referência e auxiliam
na organização das escolhas” (S23). As críticas foram pontuais e concentradas em
aspectos técnicos do MVP (como pequenos bugs ou comportamentos depreview),
e não no conteúdo conceitual do guia, o que indica que as orientações teóricas fo-
ram bem assimiladas. As sugestões de melhoria convergiram para pedidos de maior
interatividade, novos exemplos visuais e ampliação dos módulos, sinalizando não fra-
gilidades do guia, mas sim seu potencial de expansão futura.

Por fim, a intenção de reutilização (86,4%) e recomendação (93,2%) reforça o im-
pacto positivo do material e seu potencial de uso recorrente em contextos acadêmicos
e profissionais. A convergência entre dados quantitativos e qualitativos indica que o
UI4Devs não apenas foi bem recebido, mas também estimulou reflexão sobre boas
práticas de interface e apoiou de forma concreta o processo de avaliação e tomada
de decisão em design. Com poucos minutos de uso, o guia demonstrou ser capaz de
provocar aprendizado significativo, orientar escolhas visuais mais consistentes e qua-
lificar a análise crítica dos participantes, o que reforça sua relevância e aplicabilidade
no cotidiano de equipes técnicas.
8.5. AMEAÇAS ÀVALIDADE
Embora os resultados tenham sido consistentes e indiquem boa aceitação do
guia, algumas limitações metodológicas devem ser consideradas para uma interpre-
tação adequada dos achados. A coleta utilizou amostragem não probabilística por
conveniência, o que tende a concentrar respondentes com perfil da área de tecnolo-
gia. No contexto deste estudo, essa concentração era esperada e adequada, dado
que o guia foi projetado justamente para desenvolvedores e profissionais que atuam
com interfaces. Ainda assim, esse tipo de amostragem restringe a generalização dos
resultados para públicos externos ao nicho, como equipes multidisciplinares ou pro-
fissionais sem familiaridade com processos de design e desenvolvimento.
A principal limitação quantitativa decorre da diferença entre o número de parti-
cipantes que responderam ao pré-uso e aqueles que completaram o pós-uso: das
77 pessoas que iniciaram o processo, 44 concluíram ambas as etapas, resultando
em uma taxa efetiva de finalização de aproximadamente 57,1%. Para mitigar essa
perda, foram adotadas ações complementares, como o envio defollow-upspor e-mail
e mensagens via Google Chat. Além disso, ao finalizar todos os módulos do guia,
os usuários visualizaram umpopupcom lembrete explícito para acessar o formulário
de pós-uso, e uma seção adicional foi incluída no relatório final quando o progresso
atingia 100%, reforçando a chamada para resposta. Mesmo com essas estratégias,
somente as respostas completas foram consideradas na análise, assegurando con-
sistência metodológica.
Outra limitação diz respeito à ausência de controle experimental. O uso do guia
ocorreu de forma autônoma e em ambientes diversos, o que impossibilita assegurar
condições homogêneas de testagem, tempo dedicado ou nível de atenção, ou outras
variações não observáveis na experiência de uso. Além disso, a avaliação baseou-
se em uma única interação inicial com o material, o que impede observar efeitos de
uso recorrente, retenção de aprendizagem ou impacto prolongado em projetos reais.
Parte dos participantes também relatou ter apenas explorado o guia, sem aplicá-lo a
um projeto concreto, o que possivelmente reduziu a profundidade das percepções em
alguns casos.
Apesar dessas limitações, elas não comprometem a compreensão geral dos re-
sultados. Em vez disso, apontam caminhos para investigações futuras, como estudos
longitudinais, avaliações controladas em contexto profissional e testes com amostras
mais diversificadas. Esses aprofundamentos poderão ampliar a robustez da valida-
ção e explorar de maneira mais abrangente o impacto do guia em ciclos reais de
desenvolvimento.

9. CONSIDERAÇÕESFINAIS
Os resultados deste estudo demonstram que a integração entre avaliações sis-
temáticas de usabilidade e a construção de um artefato interativo fundamentado em
evidências pode apoiar desenvolvedores sem formação em design na criação de inter-
faces mais claras, consistentes e acessíveis. A análise de dois sistemas em diferentes
estágios de maturidade permitiu identificar padrões recorrentes de problemas, como
baixo contraste, ausência de feedback, inconsistências visuais e falta de orientação
contextual. Esses achados subsidiaram a elaboração do UI4Devs, um guia estrutu-
rado em quatro blocos temáticos, capaz de sintetizar princípios consagrados (Nielsen,
C.R.A.P ., WCAG e normas ISO) em recomendações objetivas e aplicáveis ao cotidi-
ano técnico. A materialização desse guia em um MVP interativo demonstrou que a
transposição das diretrizes para um ambiente guiado, modular e prático favorece a
clareza e reduz a carga cognitiva dos usuários durante a tomada de decisões de in-
terface. O artefato serviu não apenas como demonstração funcional do guia, mas
também como meio de observar, na prática, a aplicabilidade das recomendações.
A validação empírica, realizada por meio de umsurveyem duas etapas, reforçou
esses resultados. O MVP foi avaliado como claro, útil e aplicável, apresentando altas
taxas de conclusão dos módulos, tempo de uso reduzido e forte intenção de reutili-
zação e recomendação. Os participantes relataram identificar problemas que antes
não percebiam, indicando fortalecimento da capacidade analítica em UI. O alcance
geográfico diversificado e a presença de aplicações tanto em projetos reais quanto
exploratórios ampliaram a representatividade da validação, sugerindo potencial de
adoção em diferentes contextos de atuação.
Apesar desses avanços, algumas limitações metodológicas merecem considera-
ção. A amostragem por conveniência tende a concentrar o público em estudantes e
profissionais de tecnologia, reduzindo a generalização dos resultados. O uso autô-
nomo e não controlado também impede assegurar condições equivalentes entre os
participantes, e a aplicação pontual não permite observar efeitos acumulados de uso
prolongado. Além disso, parte das avaliações foi realizada sem aplicação direta em
um projeto real, o que pode limitar a profundidade de algumas percepções. Tais limi-
tações não invalidam os achados, mas indicam aspectos metodológicos que podem
ser aprimorados em investigações subsequentes.
Como continuidade deste trabalho, recomenda-se aprofundar a validação do guia
em ambientes reais de desenvolvimento, envolvendo equipes multidisciplinares e ci-
clos completos de projeto. Essa ampliação permitirá observar o comportamento do
UI4Devs em contextos colaborativos e diversificados, complementando a validação
inicial realizada de forma autônoma pelos participantes. As direções sugeridas são
coerentes com os dados coletados, especialmente na análise qualitativa, na qual sur-
giram demandas por maior interatividade, explicações mais pedagógicas, ampliação
de módulos e aprofundamento técnico das recomendações. Esses elementos refor-
çam a necessidade de evoluir o artefato para além de sua versão inicial.
A evolução natural do UI4Devs inclui a implementação completa dobackend, a
ampliação das funcionalidades do MVP e a consolidação do guia como uma plata-
forma interativa comchecklistsintegrados, trilhas personalizadas e mecanismos au-
tomáticos de verificação. Também se destaca o potencial de incorporar recursos de
inteligência artificial para sugerir ajustes visuais e auxiliar na tomada de decisão, com-

binando análise automatizada com curadoria humana. Esses caminhos ampliam o
alcance e a maturidade da solução, reforçando seu papel como recurso prático e
acessível para elevar a qualidade das interfaces produzidas por equipes técnicas.
Além dessas perspectivas, projeta-se como avanço significativo o desenvolvi-
mento de um módulo dedicado à geração automatizada depromptspersonalizados
a partir das decisões registradas ao longo dos módulos do guia. Esse recurso apoi-
aria desenvolvedores na criação de descrições mais precisas para ferramentas de
IA generativa, permitindo produzir rapidamente componentes, alternativas visuais ou
trechos de código alinhados às diretrizes definidas pelo usuário. A integração entre
dados coletados, como paleta, tipografia, padrões visuais e configurações de nave-
gação, e geração orientada por IA amplia a utilidade prática do guia e aproxima sua
aplicação de fluxos contemporâneos que combinam automação, curadoria e tomada
de decisão assistida.
DISPONIBILIDADE DEDADOS
Todos os materiais utilizados na etapa de validação do guia UI4Devs estão publi-
camente disponíveis no repositório Zenodo, garantindo transparência e possibilidade
de reuso dos dados. O conjunto inclui os formulários de pré-uso e pós-uso, as respos-
tas completas anonimizadas, os arquivos utilizados na análise quantitativa, os trechos
selecionados para a análise qualitativa e os códigos temáticos gerados no processo
de codificação. Os arquivos podem ser acessados integralmente no seguinte ende-
reço: DOI: https://doi.org/10.5281/zenodo.17796221.
REFERÊNCIAS
ALEXIOU, G.Retailers To Lose $828 Million Of Sales Over Ch-
ristmas Due To Inaccessible Websites. 2021. Disponível em:
https://www.forbes.com/sites/gusalexiou/.
BAKHSHANDEH, L. M.Defining Inclusive UX Design: Key Criteria and Industry
Insights for Creating Equitable User Experiences. [S.l.], 2025. Disponível em:
<https://digitalcommons.calpoly.edu/grcsp/299/>.
BARBOSA, S.; SILVA, B. S. da.Interação Humano-Computador e Experiência do
Usuário. 2. ed. Rio de Janeiro: Elsevier, 2021.
CAROLI, P .Lean Inception: como alinhar pessoas e construir o produto certo.
São Paulo: Editora Caroli, 2018.
CARTAXO, B.; PINTO, G.; SOARES, S. Rapid reviews in software engineering.
In: .Contemporary Empirical Methods in Software Engineering. Cham:
Springer International Publishing, 2020. p. 357–384. ISBN 978-3-030-32489-6.
Disponível em: <https://doi.org/10.1007/978-3-030-32489-6_13>.
COSTA, R. Parente da; CANEDO, E. D. A set of usability heuristics for mobile
applications. In:Design, User Experience, and Usability. [S.l.]: Springer, 2019.
DRONGELEN, M. V.; DENNIS, A.; GARABEDIAN, R.Lean Mobile App
Development: Apply Lean Startup Methodologies to Develop Successful iOS
and Android Apps. [S.l.]: Packt Publishing, 2017. ISBN 9781787120385.


GARRETT, J. J.The Elements of User Experience: User-Centered Design for the
Web and Beyond. Berkeley, CA: New Riders, 2002.
GREGOR, S.; HEVNER, A. R. Positioning and presenting design science research for
maximum impact.MIS Quarterly, v. 37, n. 2, p. 337–355, 2013.
GREGOR, S.; JONES, D. The anatomy of a design theory.Journal of the
Association for Information Systems, v. 8, n. 5, p. 312–335, 2007.
HEVNER, A.; CHATTERJEE, S. Design science research in information systems.
In: .Design Research in Information Systems: Theory and Practice.
Boston, MA: Springer US, 2010. p. 9–22. ISBN 978-1-4419-5653-8. Disponível em:
<https://doi.org/10.1007/978-1-4419-5653-8_2>.
HEVNER, A. R. et al. Design science in information systems research.MIS Quarterly,
v. 28, n. 1, p. 75–105, 2004.
ISO.ISO 9241-11:2018 – Ergonomics of human-system interaction – Part
11: Usability: Definitions and concepts. [S.l.]: International Organization
for Standardization (ISO), 2018. Acessado em: abr. 2025. Disponível em:
<https://www.iso.org/standard/63500.html>.
ISO.ISO 9241-210:2019 – Ergonomics of human-system interaction – Part
210: Human-centred design for interactive systems. [S.l.]: International
Organization for Standardization (ISO), 2019. Acessado em: abr. 2025. Disponível
em: <https://www.iso.org/standard/77520.html>.
ISO.ISO 9241-110:2020 – Ergonomics of human-system interaction
– Part 110: Interaction principles. [S.l.]: International Organization for
Standardization (ISO), 2020. Acessado em: abr. 2025. Disponível em: <https:
//www.iso.org/standard/77520.html>.
ISO/IEC.ISO/IEC 25062:2006 - Software engineering — Software product
Quality Requirements and Evaluation (SQuaRE) — Common Industry
Format (CIF) for usability test reports. [S.l.]: International Organization for
Standardization (ISO)/International Electrotechnical Commission (IEC), 2006.
<https://www.iso.org/standard/35516.html>. Acessado em: mai. 2025.
ISO/IEC.ISO/IEC 25010:2011 - Systems and software engineering —
Systems and software Quality Requirements and Evaluation (SQuaRE) —
System and software quality models. [S.l.]: International Organization for
Standardization (ISO)/International Electrotechnical Commission (IEC), 2011.
<https://www.iso.org/standard/35733.html>. Acessado em: mai. 2025.
JOHNSON, J.Designing with the Mind in Mind: Simple Guide to Understanding
User Interface Design Guidelines. Morgan Kaufmann, 2020. Disponível em:
<https://books.google.com/books?id=_dLVDwAAQBAJ>.
JOSHI, A. et al. Likert scale: Explored and explained.British Journal of Applied
Science & Technology, v. 7, n. 4, p. 396–403, 2015.
KOFFKA, K.Principles of Gestalt Psychology. New Y ork: Harcourt, Brace and
Company, 1935.


LIKERT, R. A technique for the measurement of attitudes.Archives of Psychology,
v. 22, n. 140, p. 1–55, 1932.
MAURYA, A.Running Lean: Iterate from Plan A to a Plan That Works. [S.l.]:
O’Reilly Media, 2012. ISBN 9781449305178.
MOWAR, P . et al. Codea11y: Making AI coding assistants useful for accessible
web development. In:Proceedings of the 2025 CHI Conference on Human
Factors in Computing Systems. New Y ork, NY , USA: ACM, 2025. Disponível em:
<https://doi.org/10.1145/3706598.3713335>.
NIELSEN, J.10 Usability Heuristics for User Interface Design. 1994.
<https://www.nngroup.com/articles/ten-usability-heuristics/>. Acessado em: abr.
2025.
NIELSEN, J. Severity ratings for usability problems. In: NIELSEN, J.; MACK, R. L.
(Ed.).Usability Inspection Methods. [S.l.]: John Wiley & Sons, 1994. p. 23–48.
<https://www.nngroup.com/articles/how-to-rate-the-severity-of-usability-problems/>.
NORMAN, D.; NIELSEN, J.The Definition of User Experience (UX). 2016.
Disponível em: <https://www.nngroup.com/articles/definition-user-experience/>.
OSWAL, S. K. Participatory design: Barriers and possibilities.Communication
Design Quarterly Review, v. 2, n. 3, p. 25–31, 2014.
PALOMINO, P . et al. Enhancing developers experience (devex) for successful design
system implementation.International Journal of Human–Computer Interaction,
2025.
PRODANOV, C. C.; FREITAS, E. C. D.Metodologia do trabalho científico:
métodos e técnicas da pesquisa e do trabalho acadêmico-2ª Edição. [S.l.]:
Editora Feevale, 2013.
W3C.Web Content Accessibility Guidelines (WCAG) 2.2. 2023. <https:
//www.w3.org/TR/WCAG22/>. Acessado em: abr. 2025.
WebAIM.The WebAIM Million: An annual accessibility analysis of the top
1,000,000 home pages. 2023. <https://webaim.org/projects/million/#accessibility>.
Acessado em: mai. 2025.
WILLIAMS, R.Design para quem não é designer. [S.l.]: Pearson Education do
Brasil, 2012.
WROBLEWSKI, L.Mobile First. 2011. Acessado em: mai. 2025. Disponível em:
<https://abookapart.com/products/mobile-first>.


 
 
Manoela Resende Gomes da Cunha
 
 
 
UI4DEVS: UM MVP PARA APOIAR DESENVOLVEDORES NA CRIAÇÃO DE
INTERFACES
 
 
Trabalho de Conclusão de Curso
apresentado ao Curso de Graduac
̧
ão
em Cie
̂
ncia da Computac
̧
ão da
Universidade Federal do Pampa como
requisito parcial para a obtenc
̧
ão do
título de Bacharel em Cie
̂
ncia da
Computac
̧
ão
 
 
 
 
Monografia defendida e aprovada em: 9 de dezembro de 2025.
 
Banca Examinadora:
 
____________________________________________________
Maicon Bernardino da Silveira
Orientador
 
Unipampa
 
______________________________________________________
Rafael Baldiati Parizi
Instituto Federal de Educação Ciência e Tecnologia Farroupilha (IFFAR)
 
_____________________________________________________
Amanda Meincke Melo
Unipampa
SISBI/Folha de Aprovação 1919507         SEI 23100.022065/2025-40 / pg. 1

 
Assinado eletronicamente por 
MAICON BERNARDINO DA SILVEIRA
, 
PROFESSOR DO
MAGISTERIO SUPERIOR
, em 09/12/2025, às 18:44, conforme horário oficial de Brasília, de acordo
com as normativas legais aplicáveis.
Assinado eletronicamente por 
AMANDA MEINCKE MELO
, 
PROFESSOR DO MAGISTERIO
SUPERIOR
, em 10/12/2025, às 20:47, conforme horário oficial de Brasília, de acordo com as
normativas legais aplicáveis.
Assinado eletronicamente por 
RAFAEL BALDIATI PARIZI
, 
Usuário Externo
, em 16/12/2025, às
14:17, conforme horário oficial de Brasília, de acordo com as normativas legais aplicáveis.
A autenticidade deste documento pode ser conferida no site
https://sei.unipampa.edu.br/sei/controlador_externo.php?
acao=documento_conferir&id_orgao_acesso_externo=0
, informando o código verificador 
1919507
 e o
código CRC 
34D2E73C
.
 
SISBI/Folha de Aprovação 1919507         SEI 23100.022065/2025-40 / pg. 2