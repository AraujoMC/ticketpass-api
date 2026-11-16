# Como trabalhamos em equipa

## Branches

| Branch | Dono | Para quê |
|---|---|---|
| `main` | todos | Só código que funciona. Ninguém trabalha directamente aqui. |
| `catalogo` | Araújo | Eventos/viagens e relatórios |
| `emissao` | Lesliana | Bilhetes, token e QR Code |
| `validacao` | Vassa | Validação, Redis e histórico |

## Comandos do dia a dia

```bash
# 1. Antes de começar, trazer as novidades do main
git checkout main
git pull

# 2. Ir para a tua branch e juntar as novidades
git checkout emissao          # (a tua branch)
git merge main

# 3. Trabalhar... e depois guardar
git add .
git commit -m "Emissão: criar endpoint para emitir bilhete"
git push origin emissao
```

## Juntar ao main (Pull Request)

1. No GitHub, abrir um **Pull Request** da tua branch para o `main`
2. Outra pessoa da equipa **revê o código** e aprova
3. Só depois se faz o merge

## Mensagens de commit

Curtas, no presente, começando pelo módulo: `Validação: rejeitar bilhete já utilizado`.

## Regras

- Nunca enviar senhas, chaves ou ficheiros `.env` para o GitHub
- Documentar o teu módulo à medida que o fazes
- Bloqueado? Avisa logo no grupo
