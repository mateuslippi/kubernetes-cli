# Kubernetes Pod Images Lister

Esta é uma ferramenta simples em Python para listar todas as imagens dos containers em execução nos pods do seu cluster Kubernetes.

## Pré-requisitos

- Python 3.x
- Acesso ao cluster Kubernetes configurado no seu `~/.kube/config` (kubeconfig).

## Instalação

1. Clone o repositório ou baixe o script.
2. Instale as dependências necessárias:

```bash
pip install -r requirements.txt
```

## Como usar

Para listar as imagens de todos os pods em todos os namespaces:

```bash
python kubernetes-get-images.py
```

Para listar as imagens de pods em um namespace específico:

```bash
python kubernetes-get-images.py -n <nome-do-namespace>
```

### Exemplo de Saída

A ferramenta exibirá uma tabela colorida com o nome dos pods e suas respectivas imagens.

## Tecnologias Utilizadas

- [kubernetes-python](https://github.com/kubernetes-client/python): Cliente oficial do Kubernetes para Python.
- [tabulate](https://github.com/astanin/python-tabulate): Para formatação de tabelas no terminal.
- [colorama](https://github.com/tartley/colorama): Para adicionar cores à saída do terminal.
