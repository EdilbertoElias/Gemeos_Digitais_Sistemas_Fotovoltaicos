# 🔆 Gêmeos Digitais - Sistemas Fotovoltaicos

Projeto acadêmico de simulação e análise de sistemas fotovoltaicos utilizando **MATLAB/Simulink**, implementando um gêmeo digital para estudar o comportamento de módulos fotovoltaicos sob diferentes condições de carga.

## 📋 Informações do Projeto

- **Autor**: Edilberto Elias Xavier Junior
- **Matrícula**: 120210134
- **Área**: Geração de Energia
- **Tecnologia**: MATLAB/Simulink

## 🎯 Objetivos

Este projeto implementa simulações para:

1. **Análise de Desempenho Fotovoltaico**: Estudar o comportamento de células e módulos fotovoltaicos
2. **Variação de Carga**: Simular o sistema com diferentes valores de resistência de carga (5Ω, 10Ω, 20Ω, 40Ω, 60Ω, 80Ω)
3. **Modelagem de Inversor**: Analisar o comportamento com e sem filtros de inversão de frequência
4. **Gêmeo Digital**: Criar modelos computacionais que representam o comportamento real do sistema

## 📁 Estrutura do Projeto

```
Gemeos_Digitais_Sistemas_Fotovoltaicos/
├── Projeto.m                    # Script principal de execução
├── Simulacao1.slx              # Simulação 1: Análise com variação de carga
├── Simulacao2.slx              # Simulação 2: Análise com inversor
├── Simulacao3.slx              # Simulação 3: (Análise adicional)
├── Projeto.pdf                 # Documentação do projeto
└── slprj/                       # Arquivos de projeto Simulink
```

## 🔧 Componentes Principais

### Simulacao1.slx
Analisa o desempenho do sistema fotovoltaico com **6 valores diferentes de carga resistiva**:
- Simula e coleta dados de: **Potência (kW)**, **Tensão (V)** e **Corrente (A)**
- Gera gráficos comparativos para cada condição de carga
- Exporta resultados como imagens PNG

### Simulacao2.slx
Avalia o comportamento do **inversor de frequência**:
- Analisa a saída da célula fotovoltaica (com tensão em V)
- Simula o comportamento com inversor sem filtro
- Compara comportamento antes e depois do inversor

### Simulacao3.slx
Simulação adicional para análise complementar

## 📊 Resultados Gerados

O script `Projeto.m` automaticamente gera:

- **Gráficos de Potência**: Evolução temporal da potência para cada valor de carga
- **Gráficos de Tensão/Corrente**: Análise combinada de tensão e corrente
- **Arquivos de Saída**: 
  - `Simulacao_5.png`, `Simulacao_10.png`, ... `Simulacao_80.png`
  - `Simulacao_Saida_da_Celula_Fotovoltaica.png`
  - Gráficos de inversor sem filtro

## 🚀 Como Usar

### Pré-requisitos
- MATLAB (R2021a ou superior recomendado)
- Simulink
- Toolbox de Sistemas de Potência (se necessário)

### Executar o Projeto

1. **Abra MATLAB** e navegue até a pasta do projeto:
   ```matlab
   cd 'c:\Users\edilb\Documents\GitHub\Gemeos_Digitais_Sistemas_Fotovoltaicos'
   ```

2. **Execute o script principal**:
   ```matlab
   Projeto
   ```

3. **Aguarde** a conclusão de todas as simulações (6 iterações + 2 simulações adicionais)

4. **Verifique os resultados** - imagens PNG serão geradas na pasta do projeto

### Personalizar Simulações

Para alterar os valores de resistência de carga, edite o arquivo `Projeto.m`:

```matlab
Resistencia = [5, 10, 20, 40, 60, 80];  % Valores em Ohms
```

## 📈 Métricas Coletadas

Para cada simulação são monitoradas:

| Métrica | Unidade | Descrição |
|---------|---------|-----------|
| Potência | kW | Potência instantânea gerada |
| Tensão | V | Voltagem do sistema |
| Corrente | A | Corrente elétrica |
| Tempo | s | Intervalo de simulação |

## 📚 Fundamentação Teórica

O projeto baseia-se em:
- **Modelagem de Células Fotovoltaicas**: Equações de física de semicondutores
- **Gêmeos Digitais**: Representação computacional de sistemas físicos reais
- **Análise de Sistemas de Potência**: Comportamento de inversores e filtros

Para mais detalhes, consulte o arquivo `Projeto.pdf`

## 🔍 Visualização de Dados

Os gráficos gerados mostram:
- **Seção Superior**: Evolução temporal da potência com escala automática
- **Seção Inferior**: Dual-axis com tensão (eixo esquerdo) e corrente (eixo direito)
- **Intervalo de Análise**: 0.1s a 1.0s para melhor visualização do regime permanente

## 💡 Próximos Passos / Melhorias Futuras

- [ ] Análise com diferentes irradiâncias solar
- [ ] Simulação com variação de temperatura
- [ ] Implementação de controladores MPPT (Maximum Power Point Tracking)
- [ ] Validação experimental com dados reais
- [ ] Interface gráfica para parametrização dinâmica

## 📞 Contato

**Autor**: Edilberto Elias Xavier Junior  
**Matrícula**: 120210134

---

**Última atualização**: Abril de 2025
**Status**: ✅ Completo e funcional
