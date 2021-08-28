# Introdução a JSF para aplicação web
## Pré-requisitos
- Entendimento básico da linguagem de programação em Java
- IDE
- Entendimento em tecnologias como HTML, CSS, AJAX, etc

## Projeto
1) Adição de código no `pom.xml`:
```
<properties>
	<project.build.sourceEncoding>UTF-8</project.build.sourceEncoding>
</properties>
```

2) O outro código adicionado no `pom.xml`:
```
<build>
	<finalName>${project.artifactId}</finalName>
	<pluginManagement>
		<plugins>
			<plugin>
				<artifactId>maven-compiler-plugin</artifactId>
				<version>3.1</version>
				<configuration>
					<source>1.8</source>
					<target>1.8</target>
				</configuration>
			</plugin>
		</plugins>
	</pluginManagement>
</build>
```

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
