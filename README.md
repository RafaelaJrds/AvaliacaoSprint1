<h1 align="center"> Avaliação Sprint 1


## Tema: Segurança de redes: Conheça as vulnerabilidades de servidores e clientes 
---

1. O que é um ataque DDoS e como posso me proteger? 

- <p style='text-align: justify;'> O DDoS (Distributed  Denial  of Service) é um ataque realizado em aplicações online por Hackers, que irão se aproveitar do tráfego da internet para causar a indisponibilidade do serviço, podendo paralisar a aplicação completamente ou parcialmente. O DDoS é um dos mais temidos na atualidade, pois na maioria das vezes esse tipo de ataque é bem sucedido e causa prejuízos.

    <p style='text-align: justify;'> Todos os servidores de uma aplicação online possuem uma capacidade limitada de conexões a serem recebidas pelos usuários da internet. Cientes dessa limitação, os hackers tentarão inicialmente “sequestrar” máquinas de usuários normais tornando-os um botnet (rede de hosts infetado). A partir daí, estas máquinas serão usadas para realizar um ataque que é denominado de negação de serviço distribuído, ou seja, várias máquinas de forma simultânea iniciarão conexões com o servidor-alvo, acarretando a incapacidade do mesmo de receber novas requisições de clientes reais pois todas as conexões disponíveis já foram consumidas durante o ataque, ou seja, o objetivo é comprometer o servidor-alvo enviando uma grande quantidade de tráfego que irá esgotar recursos como memória e processamento. O sequestro das máquinas que possibilita esse tipo de ataque acontecer ocorre por meio de vírus ou malware que é enviado às vítimas anteriormente.

    <p style='text-align: justify;'> Um dos motivos pelo qual esse tipo de ataque possui um alto índice de êxitové devido a dificuldade de identificar "quem" está fazendo um acesso legítimo a aplicação, já que existem diversas máquinas em diferentes locais do mundo participando da ação. 

    <p style='text-align: justify;'> Não existe uma forma que seja totalmente eficiente contra esse tipo de ataque, mas, é possível utilizar um conjunto de práticas de segurança que visam prevenir ou diminuir o impacto causado por essa falha nas organizações. 

    <p style='text-align: justify;'> Para obter êxito na segurança de redes, é necessário que as aplicações e ferramentas de segurança façam parte de um sistema. Podem ser consideradas aplicações de segurança as ferramentas de softwares executadas num dispositivo de rede, dispositivos autónomos, como routers que filtra o tráfego, IPS dedicado a prevenção, VPN responsável por criar túneis seguros encriptados, AMP, firewall que divide a rede em zonas de segurança e filtra a comunicação. No caso da DDoS é necessário que a resposta ao ataque seja em tempo real usando softwares de análise ativa que detectem o software maligno em tempo real, assim é necessário monitorar constantemente a rede buscando qualquer tipo de indícios que revelem a presença desse tipo de software. Além disso, muitas organizações adotam ainda boas práticas de segurança para prevenir esses ataques, como efetuar avaliação de riscos, implementar uma ferramenta de monitorização, analítica a gestão de redes entre outras.


2. Por que o firewall é uma ferramenta muito importante de proteção? 

- <p style='text-align: justify;'> O firewall é uma ferramenta importante para ajudar a separar redes em zonas de segurança, ele controla/filtra as comunicações que entram e saem de uma rede. O firewall torna possível selecionar o nível  de segurança da rede, fazendo com que o tráfego de requisições e respostas não aconteça da zona mínima para a de máxima segurança, essa comunicação só é possível caso a requisição tenha sido feita inicialmente pela zona de maior grau de segurança, pois o firewall tem memória stateful, ou seja, ele tem a capacidade de armazenar algumas informações como endereço IP e portas de comunicação, e ao passar pela porta ele compara e só permite a passagem caso essas informações coincidam com as armazenadas por ele.

## Tema: Git e GitHub
---
 3. Explique de forma sucinta, o fluxo e envio de um arquivo novo para o repositório do projeto. 

 - Primeiro será necessário abrir a pasta onde o arquivo está, abrir o Git Bash e digitar o comando `git init`;
 ```
 git init
 ```
  - Para verificar se o arquivo que você deseja enviar para o repósitorio está lá esperando para ser adicionado, digite o comando `git status`;
  ```
  git status
  ```
   - Para adicionar o arquivo digita-se o comando `git add .` ou `git add + "nome do arquivo"`;
   ```
   git add . 
   ```
   ou 
   ```
   git add nomedoarquivo
   ```
   - Em seguida digitar o comando `git commit -m “  ”` (entre as aspas e escrever uma mensagem que dê significado ao commit);
   ```
   git commit -m "Nome do commit"
   ```
   - Dê um `git status` para certificar se ocorreu tudo certo;
 ```
  git status
  ```
- Conecte-se com o repositório do projeto e copie o *endereço* do repositório e volte para o git bash, nele escreva o comando `git remote add origin + o endereço do repositório`
```
git remote add origin endereçodorepositório
```
- Por último envie para o repositório usando o comando `git push -u origin + nomedabranch`
```
git push -u origin nomedabranch
```
 4. <p style='text-align: justify;'> Descreva sobre os ganhos de se utilizar a funcionalidade da branch do git.

 - <p style='text-align: justify;'> Os ganhos são uma melhora na organização dos projetos, possibilitando o desenvolvimento de funcionalidades de forma separada, evita a ocorrência de bugs pois terá ao menos duas branch, (master/main e developer) uma estável e outra instável fazendo com que o software seja mais estável.

 5. Explique a diferença entre criar o repositório na nuvem e iniciar o repositório a partir de um código existente local. 

 - <p style='text-align: justify;'> Quando o repositório é criado na nuvem, basta fazer o login com a sua conta no site do repositório, em seguida escolher a opção "New repository", dar um nome a esse repositório e selecionar a opção "Createe repository". O repositório foi criado e agora os arquivos podem ser enviados para ele, nesse momento será possível escolher duas formas de enviar os arquivos, a primeira opção deverá ser feita caso não tenha sido criado um repositório local antriormente, e a segunda opção é realizar o <b>push</b> de um repositório existente, em ambos os casos o Git Bash será usado para escrever os comandos necessários para vincular o repositório local com o da nuvem. 
 - Quando um repositório é criado a partir de um código existente local, é necessário abrir o Git Bash na pasta onde o código está, e torna-lá um repositório local Git usando o comando _git init_, neste momento será criado uma pasta a mais denominada de ". git" o que demonstra que foi iniciado um novo repósitorio na pasta.

 6. Qual a diferença entre Git e GitHub?

 - <p style='text-align: justify;'> O Git é um sistema de controle de versão distribuída, ele traz segurança principalmente em trabalhos open source, em que muitas pessoas trabalham em um mesmo projeto, pois além de encriptar os arquivos, ele torna possível identificar se houve alterações no projeto, quem foi o responsável por realizar as alterações, pois ele gerencia as alterações feitas guardando um histórico, já o GitHub é uma plataforma onde é possível armazenar e compartilhar projetos para outros desenvolvedores, além de poder colaborar com projeto de outras pessoas. O GitHub usa o Git como um sistema de controle. 

 ## Tema: Fundamentos de Agilidade: seus primeiros passos para a transformação ágil 
---
 7. Quais as principais diferenças entre o modelo ágil e o waterfall (modelo em cascata)?

 - <p style='text-align: justify;'> O waterfall é mais enrijecido, por ser um modelo em cascata, só podemos passar de uma etapa para outra após a anterior ser finalizada, ou seja, as etapas a serem realizadas já são pré-definidas e dificilmente se alteram. O modelo ágil é mais flexível, trabalha por funcionalidades e não por etapas, nele a priorização das tarefas muda de acordo com as necessidades do cliente, sendo priorizadas as tarefas mais importantes e mais urgentes. Essa é a primeira diferença <b>priorização</b>.
 - <p style='text-align: justify;'> A segunda diferença é o <b>fluxo de tarefas</b>, pois, como já foi citado acima no modelo waterfall as tarefas a serem realizadas devem seguir uma ordem já definida, diferente do modelo ágil que permite alterações no fluxo de tarefas, esse fluxo sempre deve se adequar as prioridades, assim se a prioridade do projeto sofre alguma alteração, o fluxo de tarefas também deverá ser alterado.
 - <p style='text-align: justify;'> A terceira diferença é o <b>feedback</b>, como o modelo ágil trabalha por funcionalidades, acontece diversas entregas parciais do produto ao cliente, essa entrega de valor rapidamente permite identificar se o projeto está alinhado às expectativas do cliente, e caso não esteja o seu feedback será usado para aprimorar o produto. Esse processo ao final vai evitar insatisfação, desperdício de tempo e aumentará a qualidade do produto. No modelo waterfall essas entregas parciais não acontecem, o cliente só tem contato com o produto após ele ser finalizado, ou seja, não se tem feedbacks rápidos.
- Resumindo, as principais diferenças entre o modelo ágil e o waterfall são:
    - 1° Priorização
	- 2° Fluxo de tarefas
	- 3° Feedback

 8. Quais são as 3 perguntas que devem ser respondidas na Daily?

 - Devem ser respondidas as seguintes perguntas:
	- O que fez?
	- O que fará?
	- Quais problemas enfrentou?

 9. Qual o intuito das seguintes cerimônias? 

 - Daily
    - <p style='text-align: justify;'> A Daily é uma reunião diária realizada sempre no mesmo horário com duração de 15 minutos, classificada como uma reunião rápida, expositiva e objetiva, importante para auxiliar na melhoria contínua do projeto, nela são respondidas três perguntas que servirão para citar os progressos, os problemas enfrentados e as soluções encontradas durante o andamento da Sprint. Auxilia na compreensão do projeto pela equipe, além de controlar os riscos.
- Planning 
	- <p style='text-align: justify;'> É uma reunião de planejamento, e tem como objetivo definir uma Sprint Backlog, ou seja, uma lista priorizada dos itens de negócios a serem realizados, é feita a distribuição das tarefas para cada um do time de acordo com o tempo disponível. Na reunião também é formulada uma meta para a Sprint com o intuito de motivar todos da equipe. Deve durar 5% da sprint.
- Refinamento
	- <p style='text-align: justify;'> O refinamento ou zooming é realizado pelo P.O. na Product Backlog. O Product Backlog é uma lista priorizada de histórias que agrega valor para o cliente, esse processo tem como função “quebrar” essas histórias em partes menores, para organizar a lista de prioridades a serem levadas na reunião de planejamento (planning), de modo que os itens nela contido agregue valor ao projeto em desenvolvimento. Assim, o P.O. deve compreender as necessidades do cliente, identificar as histórias prioritárias do projeto, fazer a quebra das funcionalidades maiores em unidades menores, que sejam o suficiente para agregar valor ao cliente.
- Review 
	- <p style='text-align: justify;'> O review é uma reunião importante, pois nela participam todos que estão desenvolvendo o software, o time de desenvolvimento, Scrum Master, P.O., cliente e se possível o usuário. O intuito é mostrar ao cliente as funcionalidades prontas que foram desenvolvidas na Sprint, permitindo o uso do cliente ou usuário a ferramenta pronta a fim de obter o elemento mais desejado dessa reunião que é o feedback. 
- Retrospectiva 
	- <p style='text-align: justify;'> Na retrospectiva, o objetivo é identificar os pontos positivos e negativos da sprint que está sendo finalizada, descrever ações a serem feitas para a próxima sprint visando melhorias para o time e para o andamento do projeto.

10. O que é a estimativa na metodologia ágil? 
- <p style='text-align: justify;'> A estimativa na metodologia ágil consiste em avaliar todo o trabalho a ser realizado e dividi-lo no tempo disponível. As equipes que usam a metodologia ágil começassem a estimar o esforço em pontos de histórias. Na realização da estimativa toda a equipe de trabalho deve estar envolvida, pois cada membro trará uma perspectiva sobre a demanda de tempo necessário para realizar uma determinada história ao usuário.	
É importante entender que na metodologia ágil o todo do trabalho é dividido em partes menores, seguindo uma lista de priorização para determinar o fluxo de tarefas, o que facilita na realização da estimativa.

## 	Tema: Fundamentos HTTP 
---
11. O que é o protocolo HTTP? Qual a diferença entre HTTP e HTTPS? 
- <p style='text-align: justify;'> HTTP (Hypertext Transfer Protocol) é um protocolo de comunicação usado nas aplicações web para unir o cliente ao servidor, e apesar de ser independente da plataforma de desenvolvimento, existem algumas regras documentadas que devem ser seguidas. 
    <p style='text-align: justify;'> Quando o protocolo usado é o HTTP, os dados enviados entre cliente e servidor (requisição e resposta), são transmitidos em texto puro, isso faz com que seja um problema, pois esses dados estão vulneráveis, tornando possível o acesso aos dados do cliente por intermediários que também atuem nessa comunicação. Pensando nisso, foi adicionado uma camada extra de segurança no protocolo HTTP, representado pela letra S, sendo assim, no HTTPS os dados da transação são criptografados (a segurança dos dados é feita por SSL e TLS), tornando o protocolo mais seguro. O site que usa o HTTPS faz o uso de certificado digital no servidor, o qual tem a função de criar uma chave pública e uma privada usada pelo navegador para criptografar os dados que são trafegados entre cliente e servidor.

12. Cite 4 métodos HTTP
- Os métodos HTTP são:
	- **GET** : requisições (receber dados);
	- **POST**: submeter dados;
	- **PUT**: alterar um recurso
	- **DELETE**: remover um recurso 
---


    ### Principais comandos utilizados na avaliação:

-  `git init`: inicia um repositório em uma pasta local;

-  `git add`: adiciona uma alteração no diretório ativo, sinaliza ao Git que existe atualizações de um arquivo específico para serem armazenadas no próximo commit;

- `git status`: indica o estado do repositório, listando todos os arquivos que sofreram modificações desde o último commit;

- `git commit`: guarda o estado do repositório no momento atual, ou seja, grava as alterações feitas no repositório e as mensagens criadas para descrever e informar no registro log as alterações. Feito no repositório local;

- `git checkout`: Cria nova Branch, alterne entre os ramos ou restaure os arquivos da árvore de trabalho;

- `git switch --orphan` : cria uma Branch independente da principal permitindo que ela seja vazia; A partir da versão 2.23.0 do git, o comando `git checkout` pode ser substituído pelo comando `git switch`;

- `git branch`: Lista, cria ou exclui os ramos;

- `git remote`: Gerencie o conjunto de repositórios ("remotos") cujos ramos você monitora, quando usado `git remote add`, é adicionado um ramo remoto;

- `git push`: Atualiza as refs remotas utilizando as refs locais, enquanto envia os objetos necessários para que seja concluída as refs informadas;

- `git log`: Exibe os registros log do commit;

- `git commit --allow-empty`: Permite cirar um commit vazio na branch orphan;


---

### Referências bibliográficas:

- **Cursos da Alura realizada na primeira Sprint:**
    - **Fundamentos de agilidade**: Seus primeiros passos para a transformação ágil
    - **Scrum**: agilidade em seu projeto
    - **Kanban parte 1**: Fundamentos essencias
    - **Git e GitHub**: Controle e compartilhe seu código
    - **Git e GitHub**: Estratégias de ramificações, conflitos e Pull Requests
    - **HTTP**: Entendendo a Web por debaixo dos panos
    - **Segurança de redes**: Conheça as vulnerabilidades de servidores e clientes
        -Disponíveis no site: https://www.alura.com.br/ 

- **Curso de introdução à Cibersegurança da Cisco Networking Academy**
    - Disponível no site: https://www.netacad.com/pt-br/courses/cybersecurity/introduction-cybersecurity 

- **Estimativa ágil**: 
    - Disponível no site: https://itforum.com.br/noticias/como-fazer-uma-estimativa-agile-do-jeito-certo/

- **HTTPS e SSL/TLS**
    - Disponível no site: https://www.hostinger.com.br/tutoriais/o-que-e-ssl-tls-https?ppc_campaign=google_search_generic_hosting_all&bidkw=defaultkeyword&lo=1031918

- **Diferença entre Git e GitHub**:
    - Disponível: https://www.alura.com.br/artigos/o-que-e-git-github

- **Importância das Branchs**: 
    - Disponível no site: https://pt.stackoverflow.com/questions/275695/qual-a-importancia-do-branch-no-versionamento#:~:text=Branches%20separados%20ajudam%20na%20estabilidade,master%20local%20e%20o%20remoto.

- **Documentação do Git**
    - Disponível no site: https://git-scm.com/docs/git/pt_BR 

-  **Comandos do Git que você precisa conhecer** - Parte 1
    - Disponível no site: https://www.treinaweb.com.br/blog/comandos-do-git-que-voce-precisa-conhecer-parte-1

- **Comandos do Git que você precisa conhecer** - Parte 2
    - Disponível no site: https://www.treinaweb.com.br/blog/comandos-do-git-que-voce-precisa-conhecer-parte-2-repositorios-remotos

- **Como escrever uma boa mensagem de commit**
   - Disponível no site: https://devporai.com.br/como-escrever-uma-boa-mensagem-de-commit/#:~:text=Uma%20boa%20mensagem%20de%20commit%20deve%20conter%20a%20descri%C3%A7%C3%A3o%20do,voc%C3%AA%20n%C3%A3o%20trabalha%20com%20frequ%C3%AAncia.
   - Disponível no site: https://medium.com/linkapi-solutions/conventional-commits-pattern-3778d1a1e657

- **Podemos criar um branch vazio no git?**
    Disponível no site: https://comozed.com/podemos-criar-um-branch-vazio-no-git 

- **Como criar uma Branch limpa**
    - Disponível no site: https://pt.stackoverflow.com/questions/86644/como-criar-um-branch-limpo-sem-levar-o-hist%C3%B3rico-do-master-branch 

- **Branch Orphan**
    - Disponível no site: https://shannoncrabill.com/blog/git-orphan-branches/

-**Orphan branch**
    - Disponível no site: https://stackoverflow.com/questions/13969050/creating-a-new-empty-branch-for-a-new-project 

- **Git versão 2.23**
    - Disponível no site: https://github.blog/2019-08-16-highlights-from-git-2-23/

- **Git: Os novos comandos git restore e git switch**
    - Disponível no site: https://www.alura.com.br/artigos/git-os-novos-comandos-git-restore-e-git-switch

- **Repositórios remotos**
    - Disponível no site: https://docs.github.com/pt/get-started/getting-started-with-git/about-remote-repositories

- **Gerenciar branches**
    - Disponível no site: https://docs.github.com/pt/desktop/contributing-and-collaborating-using-github-desktop/making-changes-in-a-branch/managing-branches

- **Criando e enviando arquivos para seu repositório no GitHub**
    - Disponível no site: http://gabsferreira.com/criando-e-enviando-arquivos-para-seu-repositorio-no-github/#:~:text=Criando%20o%20reposit%C3%B3rio,s%C3%B3%20que%20ainda%20est%C3%A1%20vazio. 



