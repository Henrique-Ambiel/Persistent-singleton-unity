# Persistent Singleton — Unity 🎮🔄

<div align="center">

![Unity](https://img.shields.io/badge/Engine-Unity-black?style=for-the-badge&logo=unity)
![C%23](https://img.shields.io/badge/Linguagem-C%23-blue?style=for-the-badge&logo=csharp)
![Singleton](https://img.shields.io/badge/Design_Pattern-Singleton-purple?style=for-the-badge)
![Concluído](https://img.shields.io/badge/Status-Conclu%C3%ADdo-green?style=for-the-badge)

</div>
 
> Status do Projeto: ✔️ Concluído

### Tópicos

\:small_blue_diamond: [Descrição do Projeto](#descrição-do-projeto)

\:small_blue_diamond: [Funcionalidades](#funcionalidades)

\:small_blue_diamond: [Funcionamento do Sistema](#funcionamento-do-sistema)

\:small_blue_diamond: [Conceitos Aplicados](#conceitos-aplicados)

\:small_blue_diamond: [Pré-requisitos](#pré-requisitos)

\:small_blue_diamond: [Como Executar](#como-rodar-a-aplicação-arrow_forward)

\:small_blue_diamond: [Tecnologias Utilizadas](#tecnologias-linguagens-e-ferramentas)

\:small_blue_diamond: [Objetivo Acadêmico](#objetivo-acadêmico)

---

## Descrição do Projeto

Persistent Singleton é um projeto desenvolvido na Unity utilizando C#, com o objetivo de implementar o padrão de design Singleton associado à persistência de objetos entre diferentes cenas.

A implementação garante que apenas uma instância de determinado objeto permaneça ativa durante a execução do jogo, evitando duplicações e permitindo que seus dados e comportamentos continuem disponíveis durante as transições entre cenas.

O sistema também contempla o carregamento automático de Prefabs pela pasta `Resources` e a criação de uma nova instância caso não exista uma configuração previamente disponível.

## Funcionalidades

\:heavy_check_mark: Implementação do padrão de design Singleton.

\:heavy_check_mark: Verificação e gerenciamento de instâncias existentes.

\:heavy_check_mark: Carregamento de Prefabs pela pasta `Resources`.

\:heavy_check_mark: Criação automática de uma instância caso não exista um Prefab disponível.

\:heavy_check_mark: Persistência do objeto entre cenas utilizando `DontDestroyOnLoad`.

\:heavy_check_mark: Identificação e destruição de instâncias duplicadas.

## Funcionamento do Sistema

O sistema realiza o gerenciamento automático da instância do objeto seguindo uma sequência de verificações:

1. **Verificação de instância:** o sistema verifica se já existe uma instância ativa do Singleton.
2. **Carregamento de Prefab:** caso não exista uma instância, tenta localizar e carregar um Prefab correspondente na pasta `Resources`.
3. **Criação automática:** caso o Prefab não seja encontrado, um novo objeto é criado na cena e definido como instância única.
4. **Persistência entre cenas:** o método `DontDestroyOnLoad` mantém o objeto ativo durante as transições entre cenas.
5. **Controle de duplicidade:** caso uma nova instância seja criada acidentalmente, ela é destruída para preservar a instância original.

## Conceitos Aplicados

- **Singleton:** padrão de design que restringe a criação de uma classe a uma única instância acessível globalmente.
- **DontDestroyOnLoad:** método da Unity utilizado para preservar objetos durante o carregamento de novas cenas.
- **Resources:** sistema de carregamento de recursos da Unity, utilizado para localizar e instanciar Prefabs.
- **Instanciação de objetos:** criação dinâmica de objetos durante a execução do jogo.
- **Gerenciamento de instâncias:** controle da existência e unicidade de objetos durante o ciclo de vida da aplicação.

## Pré-requisitos

Para executar o projeto, são necessários:

- [Unity](https://unity.com/)
- [Visual Studio](https://visualstudio.microsoft.com/) ou outra IDE compatível com C#.

> A versão exata da Unity utilizada no desenvolvimento não foi especificada.

## Como Rodar a Aplicação \:arrow_forward:

1. Clone este repositório:

\`\`\`bash
git clone URL_DO_REPOSITORIO
\`\`\`

2. Abra o Unity Hub.

3. Selecione a opção **Add Project** e localize a pasta clonada.

4. Abra o projeto utilizando uma versão compatível da Unity.

5. Verifique a configuração do Prefab na pasta `Resources`, caso exista.

6. Execute o projeto e teste as transições entre cenas para verificar a persistência do Singleton.

## Tecnologias, Linguagens e Ferramentas

- [Unity](https://unity.com/)
- [C#](https://learn.microsoft.com/pt-br/dotnet/csharp/)
- Padrão de Design Singleton
- `DontDestroyOnLoad`
- `Resources`
- Instanciação dinâmica de objetos

## Objetivo Acadêmico

Este projeto foi desenvolvido como parte das atividades da disciplina de Estudos Avançados do curso de Jogos Digitais da PUC Campinas.

O objetivo foi aprofundar conhecimentos sobre padrões de design aplicados ao desenvolvimento de jogos, explorando técnicas de gerenciamento de instâncias, persistência de objetos e organização da arquitetura de sistemas na Unity.

---

## Licença

Licença não especificada.
