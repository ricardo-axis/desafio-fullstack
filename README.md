<h1 align="center"> Axis Challenge Fullstack Developer </h1>

<p align="center">
   <a href="#-introdução">Introdução</a> •
   <a href="#-cenário">Cenário</a> •
   <a href="#-regras-do-negócio">Regras do negócio</a> • 
   <a href="#%EF%B8%8F-funcionalidades">Funcionalidades</a> • 
   <a href="#-instruções--sugestões">Instruções & Sugestões</a> • 
   <a href="#-diferenciais-itens-opcionais">Diferenciais</a> • 
   <a href="#%EF%B8%8F-documenta%C3%A7%C3%A3o-organiza%C3%A7%C3%A3o-e-entrega">Documentação, Organização & Entrega</a> •
   <a href="#question-d%C3%BAvidas">Ajuda</a>
</p>


### 📚 Introdução

Este é um desafio `Hands-On` tem como proposito testar suas habilidades como `Fullstack Developer` e faz parte do processo seletivo da [Axis Mobfintech](https://axis-mobfintech.com/).


### 🚀 Cenário

O projeto a ser desenvolvido tem como objetivo criar uma `REST API` que atenda ao `Front-End`, de modo que permita que Correntistas de uma Cooperativa de Crédito consigam manter seus Contatos Favoritos cadastrados junto à conta corrente da cooperativa.


### 🎯 Regras do negócio

Cada contato favorito deve permitir armazenar: 

- Identificação do registro;
- Nome do contato;
- Tipo de chave pix;
  - Devem deve ser apenas: CPF, CNPJ, E-mail, Telefone ou Aleatória;
- Chave pix.

<table align="center">
	<thead>
		<tr>
			<th>Cooperativas</th>
			<th>Cooperados</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td valign = "top">
				<table>
					<thead>
						<tr>
							<th>Código</th>
							<th>Descrição</th>
						</tr>
					</thead>
					<tbody>
						<tr>
							<td>1</td>
							<td>Cooperativa A</td>
						</tr>
						<tr>
							<td>2</td>
							<td>Cooperativa B</td>
						</tr>
						<tr>
							<td>3</td>
							<td>Cooperativa C</td>
						</tr>
					</tbody>
				</table>
			</td>
			<td valign = "top">
				<table>
					<thead>
						<tr>
							<th>Cooperativa</th>
							<th>Conta Corrente</th>
							<th>Nome do Cooperado</th>
						</tr>
					</thead>
					<tbody>
						<tr>
							<td>1</td>
							<td>123456</td>
							<td>João</td>
						</tr>
						<tr>
							<td>1</td>
							<td>456789</td>
							<td>Maria</td>
						</tr>
						<tr>
							<td>1</td>
							<td>012348</td>
							<td>Pedro</td>
						</tr>
						<tr>
							<td>2</td>
							<td>129</td>
							<td>Luana</td>
						</tr>
						<tr>
							<td>2</td>
							<td>328</td>
							<td>Júlia</td>
						</tr>
						<tr>
							<td>3</td>
							<td>129</td>
							<td>Gumarães</td>
						</tr>
						<tr>
							<td>3</td>
							<td>456789</td>
							<td>Fonseca</td>
						</tr>
						<tr>
							<td>3</td>
							<td>885544</td>
							<td>Carol</td>
						</tr>
					<tbody>
				</table>
			</td>
		</tr>
	</tbody>
</table>


### ⚙️ Funcionalidades

A API deve fornecer serviços REST para que o Front-End consiga: 

 - pesquisar, incluir, alterar e/ou atualizar e excluir (lógica) as Cooperativas;
 - pesquisar, incluir, alterar e/ou atualizar e excluir (lógica) os Cooperados;
   - a pesquisa do cooperado pode ser por conta corrente ou nome do cooperado.
 - pesquisar, incluir, alterar e/ou atualizar e excluir (física) os seus Contatos Favoritos.

**Importante**: lembre-se de usar os verbos Https corretamente.


### 📌 Instruções & Sugestões

Espera-se que:
- Seja utilizado [linguagem C#](https://docs.microsoft.com/pt-br/dotnet/csharp/tour-of-csharp/) e [.NET8.0](https://dotnet.microsoft.com/en-us/download/dotnet/8.0) (ou [superior](https://dotnet.microsoft.com/en-us/download/dotnet));
- Boas práticas de programação orientação a objetos e conceitos de SOLID;
  - Lembre-se de alguns conceitos de design e/ou arquitetura: DDD, CQS, CQRS, Clean, Onion, Hexagonal, etc. de como organiza seu do código fonte.
  Entretando, leve em consideração ainda mais o que acredita melhor para este projeto como um todo perante os desafios, experiências e oportunidades que já foram compartilhados com você;
- Seja utilizado um banco de dados como [PostgreSQL](https://www.postgresql.org/download/), ou [SQL Server](https://www.microsoft.com/pt-br/sql-server/sql-server-downloads), ou [Oracle](https://www.oracle.com/br/database/technologies/xe-downloads.html), etc. para armazenamento dos dados;
  - Recomendável usar drivers oficiais para integração com o DB;
  - Além da criação do Banco de Dados e Tabelas usando o conceito de Code First (se souber), crie também os scripts SQL das tabelas para armazenar os dados da Cooperativa, Conta Corrente e Contatos Favoritos, bem como os scripts para alimentar o seu banco de dados;
- Para o Front-End as telas devem ser construídas preferencialmente com o framework [ReactJS](https://react.dev/).
  

### 💡 Diferenciais (itens opcionais)

- Escrever `Unit Tests`, `Integration Tests` ou `End-to-End` para os serviços de `back-end` e/ou `front-end`;
- Escrever a `Documentação da API` utilizando o conceito de `Open API 3.0`;
  - Podem ser utilizadas opções como Swagger, Redoc, Elements, RapidDoc, WidderShin, Lucybot, etc.
- Padronizar as mensagens de retorno da API em caso de sucesso e/ou erros para facilitar a organização do `front-end`.
- Configurar `Dockerfile` e/ou `Docker Compose` no projeto para facilitar o `Deploy` da equipe de `DevOps`;
  - Deploy em algum servidor, com ou sem automatização do CI;
- Configurar um sistema de alerta se houver algum falha na aplicação;


### ✔️ Documentação, Organização e Entrega

- Para a entrega abra um `Pull Request` para a branch `main` para análise e possível aprovação.
- Crie um arquivo `ENTREGA.md` contendo:
  - A lista de frameworks e/ou tecnologias usadas;
  - Instruções de como instalar e executar cada um dos projetos (front-end e back-end);
- Não esqueça do arquivo no repositório [.gitignore](https://www.toptal.com/developers/gitignore) para não subir "sujeita".
- O **prazo limite para entrega deste desafio termina em 27/03/2025 às 23h59min**.
  - ***Obs.**: as entregas realizadas após este limite não serão validadas. Apenas os commits feitos até o prazo estabelecido.*



### :question: Dúvidas?

- Ficou com alguma dúvida sobre o desafio? Entre em contato abrindo um [Issue](https://github.com/ricardo-axis/desafio-fullstack/issues) que nós te ajudaremos com o processo.
