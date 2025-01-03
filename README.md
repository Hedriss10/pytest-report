# pytest-report

```markdown
Uma biblioteca para gerar relatórios de testes com emojis de maneira simples e estilizada!

## 🚀 Instalação

Você pode instalar o `pytestreport-md` diretamente do PyPI usando o pip:

# bash
pip install pytestreport-md
```

## 📄 Descrição

O `pytestreport-md` é uma biblioteca leve que facilita a geração de relatórios de testes em formato Markdown. Ele transforma os resultados de testes em relatórios estilizados, incluindo emojis para indicar o status de cada teste (✅ para aprovados e ❌ para falhos).

## 🛠️ Como Usar

Aqui está um exemplo básico de uso:

```python
from pytestreport.reporter import generate_report_pytest

test_results = """
TestExample1 - PASSED | TestExample2 - FAILED | TestExample3 - PASSED
"""

generate_report_pytest(prefix="Name project", test_results=test_results, output_path="report.md")
```

### Resultado

Um arquivo `report.md` será gerado com um relatório detalhado:

```
## Test Report - `Name project`

--------------------------------------------------
### 📝 Test results

**Total Tests**: 3  
**Passed**: 2  
**Failed**: 1  

### Passed Tests ✅
- TestExample1
- TestExample3

### Failed Tests ❌
- TestExample2

--------------------------------------------------
### 📊 Test Summary

- **Passed Tests**: 2 ✅
- **Failed Tests**: 1 ❌

---
_Report styled with ❤️ for `Name project` on 01-Jan-2025 at 10:00:00_
```

## ⚙️ Configuração Adicional

Se necessário, você pode personalizar o comportamento da função `generate_report_pytest`:

- **`prefix`**: Colocar o nome do projeto que você está utilizando no relatório de teste.
- **`test_results`**: Resultados dos testes no formato `<nome do teste> - <status>`, separados por `|`.
- **`output_path`**: Caminho para salvar o relatório Markdown (por padrão, `report.md` será criado no diretório atual).

## 🧪 Testes

Para rodar os testes do projeto:

```bash
pytest
```

Certifique-se de estar no ambiente virtual configurado e que as dependências de desenvolvimento estejam instaladas.

## 📝 Licença

Este projeto está licenciado sob os termos da licença MIT. Veja o arquivo [LICENSE](LICENSE) para mais detalhes.

## 📬 Contribuições

Contribuições são bem-vindas! Sinta-se à vontade para abrir issues ou enviar pull requests no [repositório do projeto](https://github.com/Hedriss10/pytest-report).

## 📚 Recursos

- **Repositório**: [GitHub](https://github.com/Hedriss10/pytest-report)
- **PyPI**: [pytestreport-md](https://pypi.org/project/pytestreport-md/)

---

Feito com ❤️ por [Hedris Pereira](https://github.com/Hedriss10)

