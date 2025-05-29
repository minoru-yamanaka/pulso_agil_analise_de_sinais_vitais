# 📊 Pulso Ágil - Análise de Sinais Vitais

Sistema automatizado para análise e interpretação clínica de sinais vitais, com geração de relatórios em PDF.

## 🩺 Funcionalidades

- **Coleta de dados**: Interface interativa para inserção de valores iniciais e novos valores dos sinais vitais
- **Análise comparativa**: Cálculo automático de alterações percentuais entre medições
- **Interpretação clínica**: Avaliação automática do estado do paciente baseada em padrões clínicos
- **Geração de relatórios**: Exportação dos resultados em formato PDF profissional
- **Validação de parâmetros**: Classificação automática dos valores como Normal, Alto ou Baixo

## 📋 Parâmetros Monitorados

| Parâmetro | Faixa Normal |
|-----------|--------------|
| SpO₂ (Saturação de O₂) | 95-100% |
| Frequência Cardíaca | 60-100 bpm |
| Pressão Sistólica | 90-130 mmHg |
| Pressão Diastólica | 60-90 mmHg |
| Frequência Respiratória | 12-20 rpm |
| Pulso | 60-100 bpm |

## 🏥 Interpretações Clínicas Automáticas

O sistema identifica automaticamente as seguintes condições:

- **Comprometimento Pulmonar**: SpO₂ < 95% + FR > 20
- **Choque Circulatório/Desidratação**: FC > 100 + PA baixa
- **Estresse/Dor/Febre**: FC e FR elevadas + PA normal
- **Estado Estável**: Todos os parâmetros dentro da normalidade

## 🚀 Instalação

### Windows (Jupyter Notebook)
```bash
pip install matplotlib reportlab pandas
```

### Google Colab
```python
!pip install reportlab
# matplotlib e pandas já estão instalados
```

### Instalação Completa (todos os ambientes)
```bash
pip install matplotlib reportlab pandas
```

## 💻 Como Usar

1. **Execute o script**:
   ```python
   python analise_sinais_vitais.py
   ```

2. **Insira os valores iniciais** quando solicitado:
   - SpO₂
   - Frequência Cardíaca
   - Pressão Sistólica
   - Pressão Diastólica
   - Frequência Respiratória
   - Pulso

3. **Insira os novos valores** para comparação

4. **Visualize os resultados** no terminal

5. **Acesse o relatório PDF** gerado automaticamente

## 📄 Exemplo de Saída

```
📊 Resultado da Análise dos Sinais Vitais:

Parâmetro                 Valor Inicial  Novo Valor  Status   % Alteração
SpO2                           98.0        94.0      Baixo       -4.08%
Frequência Cardíaca            72.0        88.0     Normal       22.22%
Pressão Sistólica             120.0       110.0     Normal       -8.33%
Pressão Diastólica             80.0        75.0     Normal       -6.25%
Frequência Respiratória        16.0        22.0       Alto       37.50%
Pulso                          72.0        88.0     Normal       22.22%

🩺 Interpretação Clínica:
Comprometimento pulmonar (SpO₂ baixa + FR alta)
```

## 📁 Estrutura do Projeto

```
├── analise_sinais_vitais.py    # Script principal
├── analise_sinais_vitais.pdf   # Relatório gerado automaticamente
└── README.md                   # Documentação
```

## 🛠️ Tecnologias Utilizadas

- **Python 3.x**
- **Pandas**: Manipulação e análise de dados
- **ReportLab**: Geração de relatórios PDF
- **Matplotlib**: Visualização de dados (dependência)

## 📊 Recursos do Relatório PDF

- Layout profissional em formato A4
- Tabela formatada com todos os parâmetros
- Percentuais de alteração calculados automaticamente
- Interpretação clínica destacada
- Formatação com fontes e espaçamento otimizados

## ⚠️ Importante

Este sistema é uma ferramenta de apoio educacional e não substitui a avaliação médica profissional. Sempre consulte um profissional de saúde qualificado para interpretação clínica definitiva.

## 🤝 Contribuições

Contribuições são bem-vindas! Sinta-se à vontade para:
- Reportar bugs
- Sugerir melhorias
- Adicionar novos parâmetros
- Melhorar as interpretações clínicas

## 📝 Licença

Este projeto está sob a licença MIT. Veja o arquivo `LICENSE` para mais detalhes.

---

**Desenvolvido para auxiliar profissionais de saúde e estudantes na análise sistemática de sinais vitais.**