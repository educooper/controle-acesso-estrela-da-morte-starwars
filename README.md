<h1 align="center">Controle de Acesso da Estrela da Morte  - STARWARS</h1>
<p align="center">
<img src="https://github.com/educooper/controle-acesso-estrela-da-morte-starwars/raw/main/nave.png" alt="nave" height="120px" width="120px" />
  </p>

<p align="center">
  <img alt="Github top language" src="https://img.shields.io/github/languages/top/educooper/controle-acesso-estrela-da-morte-starwars?color=green"> 
  <img alt="Github language count" src="https://img.shields.io/github/languages/count/educooper/controle-acesso-estrela-da-morte-starwars?color=56BEB8">
 <img alt="Repository size" src="https://img.shields.io/github/repo-size/educooper/controle-acesso-estrela-da-morte-starwars?color=56BEB8">

 

<hr>



<p align="center">
  <a href="#dart-about">About</a> &#xa0; | &#xa0; 
  <!-- <a href="#sparkles-features">Features</a> &#xa0; | &#xa0; -->
  <a href="#rocket-technologies">Technologies</a> &#xa0; | &#xa0;
  <a href="#white_check_mark-requirements">Requirements</a> &#xa0; | &#xa0;
  <a href="#checkered_flag-starting">Starting</a> &#xa0; | &#xa0;
  <!-- <a href="#memo-license">License</a> &#xa0; | &#xa0; -->
  <a href="https://github.com/educooper" target="_blank">Author</a>
</p>

<br>

## :dart: About / Sobre ##

Aplicação de Curso sobre modelagem de Banco de dados baseado em SQL Server com tema Star Wars almejando a um controle de acesso REST de pilotos para naves com pesquisa e relacionamentos com base nos dados de [SWAPI - The Star Wars API](https://swapi.dev/) - Adicionado tabelas e relacionamentos sobre filmes.

## :rocket: Technologies / Tecnologias ##

Usou-se neste projeto:

- .NET Core
- C#
- SQL
- SQLSERVER

## :white_check_mark: Requirements / Requisitos ##

Antes de iniciar :checkered_flag:, você precisa ter instalado o [Git](https://git-scm.com) e .NET Core.

## :checkered_flag: Starting / Início ##

```bash
# Clone este projeto
$ git clone https://github.com/educooper/controle-acesso-estrela-da-morte-starwars

# Acesse
$ cd dio-contas-bancarias

# Execute o projeto
$ dotnet run
```

## :coffee: Addicional Features / Recursos Adicionais 

```sql
****** Filmes *****************************************************************************

CREATE TABLE Filmes(
	idFilme int NOT NULL,
	Titulo varchar(250) NOT NULL,
	idEpisodio int NOT NULL,
	DtLancamento datetime NULL,

)
GO
ALTER TABLE Filmes ADD CONSTRAINT PK_Filmes PRIMARY KEY (IdPiloto)

GO
ALTER TABLE Filmes  ADD CONSTRAINT FK_Filmes_Planeta FOREIGN KEY(IdPlaneta)
REFERENCES Planetas (IdPlaneta)

GO
ALTER TABLE Filmes  ADD CONSTRAINT FK_Filmes_Pilotos FOREIGN KEY(IdPiloto)
REFERENCES Pilotos (IdPiloto)

GO
ALTER TABLE Filmes  ADD CONSTRAINT FK_Naves_Naves FOREIGN KEY(IdNave)
REFERENCES Naves (IdNave)
********************************************************************************************
```



<a href="#top">Voltar ao Topo</a>

