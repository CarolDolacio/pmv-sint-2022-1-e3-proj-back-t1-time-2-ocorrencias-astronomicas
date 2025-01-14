# Especificações do Projeto

Tendo em vista que atualmente o usuário interessado em informações astronômicas depara-se com a dificuldade em encontrar uma fonte de informação, o projeto busca desenvolver uma aplicação web que contenha dados quanto à, ocorrências astronômicas, baseadas na localização informada pelo usuário.

Assim, neste documento serão abordadas as definições de persona, histórias de usuários, requisitos funcionais e não funcionais além das restrições do projeto utilizando técnicas de obtenção de dados, como questionários online, para compreender de forma específica nosso usuário e suas necessidades.

## Personas

<table>
  <tr>
    <th>Foto</th>
    <th>Nome</th>
    <th>Descrição</th>
    <th>Aplicativos</th>
    <th>Motivações</th>
    <th>Frustrações</th>
    <th>Hobbies, História</th>
  </tr>
  <tr>
    <td><img title="Jose Augusto" src="https://i.imgur.com/APc56HT.jpg"/></td>
    <td>José Augusto</td>
    <td>
      <ul>
        <li>13 anos</li>
        <li>Estudante do ensino fundamental</li>
        <li>Mora no interior de SP</li>
      </ul>
    </td>
    <td>
      <ul>
        <li>Facebook</li>
        <li>Instagram</li>
        <li>Youtube</li>
        <li>Tik Tok</li>
      </ul>
    </td>
    <td>
      <ul>
        <li>Revista Recreio</li>
        <li>Felipe Neto</li>
        <li>Astronautas</li>
      </ul>
    </td>
    <td>
      <li>Não sabe muito sobre cometas</li>
      <li>Nunca viu fenômenos astronômicos</li>
      <li>Quer aprender bateria</li>
    </td>
    <td>
      <li>Ler revista Recreio</li>
      <li>Filmes de ação e ficção científica</li>
      <li>Recentemente, descobriu que gosta muito da NASA, Space X e de astros, então quer aprender mais sobre</li>
    </td>
  </tr>
  <tr>
    <td><img title="Maria Eugênia" src="https://i.imgur.com/EZmVbet.jpg"/></td>
    <td>Maria Eugênia</td>
    <td>
      <ul>
        <li>31 anos</li>
        <li>Artista</li>
        <li>Mora no Rio de Janeiro</li>
      </ul>
    </td>
    <td>
      <ul>
        <li>Twitter</li>
        <li>Instagram</li>
        <li>Youtube</li>
      </ul>
    </td>
    <td>
      <ul>
        <li>Frida Kahlo</li>
        <li>Tarsila do Amaral</li>
        <li>Rihanna</li>
      </ul>
    </td>
    <td>
      <li>Não sabe quando vai ter algum fenômeno astronômico</li>
      <li>Não sabe o que está vendo no espaço</li>
      <li>Quer fazer quadros mais detalhados do espaço</li>
    </td>
    <td>
      <li>Fotografia</li>
      <li>Música</li>
      <li>Desde que comprou um telescópio não conseguiu tirar os olhos do céu, porém ela nunca sabe quando vai ocorrer
        cada evento astronômico e se será capaz de vê-los</li>
    </td>
  </tr>
  <tr>
    <td><img title="Renato Luís" src="https://i.imgur.com/rGQVtoe.jpg" /></td>
    <td>Renato Luís</td>
    <td>
      <ul>
        <li>56 anos</li>
        <li>Professor de Ciências</li>
        <li>Mora em Belo Horizonte</li>
      </ul>
    </td>
    <td>
      <ul>
        <li>Youtube</li>
        <li>Facebook</li>
        <li>Reddit</li>
      </ul>
    </td>
    <td>
      <ul>
        <li>Coisa de Nerd(Leon e Nilse)</li>
        <li>Elon Musk</li>
        <li>NASA</li>
      </ul>
    </td>
    <td>
      <li>Não encontra sites bons sobre astronomia</li>
      <li>Não consegue engajar os alunos</li>
      <li>Pensa em comprar telescópio, mas antes quer saber se vai conseguir ver vários fenômenos</li>
    </td>
    <td>
      <li>Música</li>
      <li>Barzinho com os amigos</li>
      <li>Dar aulas criativas</li>
      <li>Ele deseja que seus alunos se interessem mais por astronomia, mas tem dificuldade de encontrar plataformas
        para isso</li>
    </td>
  </tr>
  <tr>
    <td><img title="Eduardo"
        src="https://images.generated.photos/4kl3NFu9b1hfPOPq4U4gvFCE0HG_PEdFj2CQDhKK4WQ/rs:fit:512:512/wm:0.95:sowe:18:18:0.33/Z3M6Ly9nZW5lcmF0/ZWQtcGhvdG9zL3Ry/YW5zcGFyZW50X3Yz/L3YzXzAzMTg5ODYu/cG5n.png"/></td>
    <td>Eduardo</td>
    <td>
      <ul>
        <li>77 anos</li>
        <li>Engenheiro aposentado</li>
        <li>Mora no interior de Minas</li>
      </ul>
    </td>
    <td>
      <ul>
        <li>Facebook</li>
        <li>G1</li>
      </ul>
    </td>
    <td>
      <ul>
        <li>Jornais</li>
        <li>Space X</li>
        <li>Bill Gates</li>
      </ul>
    </td>
    <td>
      <li>Tem muito tempo livre nas mãos</li>
      <li>Quer aprender mais coisas</li>
    </td>
    <td>
      <li>Ler jornais</li>
      <li>Passar tempo com seus netos</li>
      <li>Assistir tv</li>
      <li>Desde que se aposentou começou a se interessar mais pela astronomia, então quer encontrar um site que o ajude
        a entender mais</li>
    </td>
  </tr>
</table>

## Histórias de Usuários

|EU COMO... `PERSONA`| QUERO/PRECISO ... `FUNCIONALIDADE` |PARA ... `MOTIVO/VALOR`                 |
|--------------------|------------------------------------|----------------------------------------|
|Como usuário   | Quero poder verificar as ocorrências astronômicas de acordo com a localização.           | Para que eu tenha conhecimento de que ocorrências eu posso visualizar em minha localidade.              |
|Como usuário       | Quero poder verificar informações sobre ocorrências astronômicas                 | Para que eu possa entender seus conceitos e o que cada termo significa. |
|Como usuário       | Quero poder postar comentários visíveis para outros usuários.                    | Para que eu possa compartilhar conhecimento com outras pessoas interessadas em ocorrências astronômicas. |
|Como usuário       | Quero poder visualizar os comentários de outros usuários.                 | Para que eu possa adquirir novos conhecimentos. |
|Como usuário       | Quero poder me cadastrar no site.                 |Para poder salvar e acessar minhas informações e dados independente do lugar ao qual o site for acessado.|
|Como usuário       | Quero poder salvar imagens de ocorrências astronômicas visíveis para outros usuários.                 | Para poder ver e compartilhar novas imagens sobre ocorrências astronômicas. |

## Requisitos

As tabelas que se seguem apresentam os requisitos funcionais e não funcionais que detalham o escopo do projeto.

### Requisitos Funcionais

|ID    | Descrição do Requisito  | Prioridade |
|------|-----------------------------------------|----|
|RF-001| Permitir o cadastro  do usuário na plataforma   | ALTA |
|RF-002| Permitir login de usuários cadastrados   | ALTA |
|RF-003| Permitir o salvamento dos dados cadastrados no banco de dados   | ALTA |
|RF-004| Permitir ao usuário inserir comentários visíveis a outros usuários    | MÉDIA |
|RF-005| Permitir ao usuário inserir fotos visíveis a outros usuários    | MÉDIA |
|RF-006| Permitir busca por palavra-chave referente a ocorrência astronômica   | MÉDIA |
|RF-007| Tela informativa sobre ocorrências astronômicas   | MÉDIA |
|RF-008| Apresentar calendário de ocorrências astronômicas   | MÉDIA |
|RF-009| Permitir que o usuário visualize ocorrências astronômicas visíveis   | MÉDIA |
|RF-010| Será possível visualizar em uma página os integrantes do grupo    | BAIXA |
|RF-011| Ao clicar na logo deverá ser redirecionado a página inicial    | MÉDIA |
|RF-012| Ao executar o scroll na tela inical deve ser levada para a tela de eventos astronômicos   | MÉDIA |

### Requisitos não Funcionais

|ID     | Descrição do Requisito  |Prioridade |
|-------|-------------------------|----|
|RNF-001| O sistema deve ser web | MÉDIA | 
|RNF-002| O sistema será desenvolvido em HTML5, CSS3 e JS | MÉDIA | 
|RNF-003| Utilização do Banco de Dados para armazenamento dos dados inseridos pelo usuário | MÉDIA | 
|RNF-004| A aplicação web será estruturada utilizando ASP.NET MVC  | MÉDIA | 

## Restrições

O projeto está restrito pelos itens apresentados na tabela a seguir.

|ID| Restrição                                             |
|--|-------------------------------------------------------|
|01| O projeto deverá ser entregue até o final do semestre |
|02| Deve ter o back-end desenvolvido        |
|03| Deve ter o front-end desenvolvido de forma intuitiva e utilizando dos conceitos de UI/UX       |

## Diagrama de Casos de Uso

<img src="img/Diagrama de caso de uso - Página 1.png"/>
