<!-- Título -->
# Base Flutter Project — Architecture MVP

Este projeto serve como uma base sólida para desenvolvedores Flutter que desejam implementar a arquitetura **MVP (Model-View-Presenter)** em seus aplicativos.

A arquitetura MVP organiza o código de maneira a separar responsabilidades, garantindo que a lógica de negócios fique isolada da interface do usuário e facilitando testes, manutenção e evolução do projeto.

## Objetivo do Projeto

* **Modularidade:** Prover uma estrutura bem definida para organizar pastas e arquivos de forma escalável.

* **Manutenção:** Facilitar a manutenção e a evolução do aplicativo, permitindo alterações rápidas em qualquer camada sem impactos inesperados.

* **Testabilidade:** Suporte para testes unitários e de integração, assegurando a confiabilidade do aplicativo.

* **Reutilização do Código:** Possibilitar o uso de componentes reutilizáveis em diferentes partes do aplicativo.

* **Separação de Responsabilidades**: Implementar um padrão claro onde:
  * **Model:** Gerencia os dados e a lógica de negócios.
  * **View:** Exibe os dados e interage com o usuário.
  * **Presenter:** Faz a ponte entre a Model e a View, controlando o fluxo de dados e as interações do usuário.

## Estrutura de Pastas e Arquivos

A estrutura é organizada para refletir claramente a arquitetura MVP:

* lib:
  * core:
    * constants
    * utils
    * partials
    * services
  * feature:
    * feature_name:
      * data:
        * models
        * repositories
      * presentation:
        * views
        * presenters
      * tests
  * app:
    * routes
    * di
    * app.dart
  * main.dart

### Explicação da Pasta `core`

Ela é uma parte fundamental da estrutura do projeto, destinada a conter recursos globais e reutilizáveis que não estão diretamente ligados a uma funcionalidade especifica.

Seu objetivo principal é centralizar e organizar elementos comuns do aplicativos, promovendo reutilização, manutenção simplificada e redução de código duplicado.

### Subpastas e Suas Funções

#### Constants

* Contém valores imutáveis e configurações que são usados em todo o aplicativo, como:
  * **Strings constantes:** Textos usados repetidamente.
    * Exemplo: mensagens de erro, rótulos de botões, etc.
  * **Cores:** Paleta de cores padronizada.
  * **Temas:** Configurações de estilo do aplicativo.
    * Exemplo: fontes, espaçamentos, etc.
  * **Dimensões:** Valores de layout fixos, como margens e paddings.

#### Utils

* Contém funções auxiliares ou classes utilitárias que não pertencem a uma funcionalidade especifica:
  * Formatação de datas ou números.
  * Manipulação de strings, como truncar, capitalizar.
  * Validação de entradas do usuário.

#### Partials

* Armazena widgets reutilizáveis que podem ser usados em várias telas ou recursos do aplicativo.
* São componentes independentes e genéricos, como:
  * Botões customizados.
  * Inputs de texto estilizados.
  * Spinner ou indicadores de carregamento.

#### Services

* Inclui serviços globais ou classes que lidam com funcionalidades como:
  * Armazenamento local.
    * Exemplo: cache, banco de dados.
  * Configuração de analytics ou notificações.
* Essa pasta também pode conter interfaces e implementações que seguem o princípio da injeção de dependência.

<!-- Informações -->
## &#8505; Informações

![Visitors](https://api.visitorbadge.io/api/visitors?path=Devsgeeknerd%2Fbas-flu-pro-mvp-pro-pro&label=Visitantes&labelColor=%23700070&labelStyle=none&countColor=%23000fff&style=plastic&color=%23ffffff "Total de Visitantes")
&nbsp;
![Followers](https://img.shields.io/github/followers/Devsgeeknerd?style=p&label=Seguidores&labelColor=800080&color=000fff "Total de Seguidores")
&nbsp;
![Watchers](https://img.shields.io/github/watchers/Devsgeeknerd/bas-flu-pro-mvp-pro-pro?style=p&label=Observadores&labelColor=800080&color=000fff "Total de Observadores")
&nbsp;
![Stars](https://img.shields.io/github/stars/Devsgeeknerd/bas-flu-pro-mvp-pro-pro?style=p&label=Estrelas&labelColor=800080&color=000fff "Total de Estrelas")
&nbsp;
![Forks](https://img.shields.io/github/forks/Devsgeeknerd/bas-flu-pro-mvp-pro-pro?style=p&label=Bifurcações&labelColor=800080&color=000fff "Total de Bifurcações")
&nbsp;
![Repo Size](https://img.shields.io/github/repo-size/Devsgeeknerd/bas-flu-pro-mvp-pro-pro?style=p&label=Tamanho&labelColor=800080&color=000fff "Tamanho do Repositório")
&nbsp;
![License](https://img.shields.io/github/license/Devsgeeknerd/bas-flu-pro-mvp-pro-pro?style=p&label=Licença&labelColor=800080&color=000fff "Licença do Repositório")
