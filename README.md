# 🎼 Chord Notes Finder 🎸

Uma ferramenta prática para decompor cifras e visualizar as notas que compõem cada acorde.

---

## 🎵 Sobre o Projeto
Este projeto foi desenvolvido para músicos e programadores que precisam identificar rapidamente a estrutura harmônica de um acorde. Ao inserir uma **cifra**, o sistema retorna as **notas** correspondentes.

### Ícones de Referência:
* **Partitura:** 🎼 (`:musical_score:`)
* **Cifra:** 🎸 (`:guitar:`) ou 🎹 (`:keyboard:`)

---

## 🚀 Como Funciona?
O motor do código utiliza lógica de intervalos musicais para calcular as notas a partir da tônica.

### 📋 Exemplo de Retorno:
Se você buscar pelo acorde **G7 (Sol com Sétima Dominante)**:

| Cifra | Notas | Estrutura |
| :--- | :--- | :--- |
| **G7** | G, B, D, F | T - 3M - 5J - 7m |

---

## 💻 Exemplo de Código (Python)
Aqui está uma demonstração de como o código processa a escala:

```python
def obter_notas_acorde(cifra):
    # Exemplo simplificado de mapeamento
    dicionario_acordes = {
        "C": ["C", "E", "G"],
        "Am": ["A", "C", "E"],
        "G7": ["G", "B", "D", "F"]
    }
    return dicionario_acordes.get(cifra, "Acorde não encontrado")

print(f"🎼 Notas de G7: {obter_notas_acorde('G7')}")
