# Introdução a JSF para aplicação web
## Pré-requisitos
- Entendimento básico da linguagem de programação em Java
- IDE
- Entendimento em tecnologias como HTML, CSS, AJAX, etc

## @RequestScoped
É o escopo padrão caso você não informe um, ele funciona como um simples HTTP request, é descartado ao fim de cada requisição, o ManagedBean não manterá seu estado entre as solicitações/requisições HTTP que o usuário fizer. A cada requisição uma nova instância do ManagedBean será criada, usada e descartada, dessa maneira não há compartilhamento das informações do ManagedBean entre as requisições. 

## @ViewScoped
É um tipo de escopo que fica entre o RequestScoped e o SessionScoped. O ManagedBean vai manter o seu estado enquanto o usuário permanecer na mesma página. Qualquer navegação para outra página ou até mesmo um um redirect para a mesma página ocasionará o fim do ManagedBean. 

## @SessionScoped 
É o escopo padrão caso você não informe um, ele tem o mesmo comportamento da sessão web (HttpSession), o estado do ManagedBean é mantido até o fim da sessão do usuário. É preciso ter muito cuidado ao utilizar o SessionScoped, pois ele será mantido em memória até que o usuário termine a sessão.

## @ConversationScoped
Só pode ser usado com CDI e controle é feito manualmente, ele funciona basicamente como uma transação de banco de dados. São necessários comandos para iniciar e para finalizar o seu ciclo de vida. O ManagedBean do tipo ConversationScoped tem apenas dois estados, transient e long running. O estado será transient antes do início e após o fim da conversação.

## @ApplicationScoped
Funciona como um Singleton, ou seja, mantém apenas uma única instância na memória em toda a aplicação, todo usuário tem acesso ao mesmo ManagedBean, logo não é aconselhável guardar informações de usuário com ApplicationScoped. 

## Dependent
Só pode ser usado com CDI, este escopo não possui um comportamento próprio, ele vai herdar o comportamento do ManagedBean em que for injetado.

## NoneScoped
Dura apenas uma chamada da EL e depois é eliminado da memória. É um escopo extremamente curto, e será usado em tarefas muito específicas.  

## Java EE
É uma plataforma padrão para desenvolver aplicações Java de grande porte e/ou para a internet.

## Especificações
- Java Servelets
- JSP
- JPA
- EJB
- JSF

## JSF
JavaServer Faces (JSF) é um web framework MVC que simplifica a construção de User Interface (UI) baseadas em componentes para aplicações web. Principais frameworks: PrimeFaces, RichFaces, ICEfaces.
