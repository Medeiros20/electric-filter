# 🎛️ Audio Spectrum Analyzer & Low-Pass Filter Simulation

> Um projeto de Processamento Digital de Sinais (DSP) que simula o comportamento de um circuito RC Passa-Baixa para isolar frequências graves de uma mistura de áudios.

![Python](https://img.shields.io/badge/Python-3.8%2B-blue)
![Librosa](https://img.shields.io/badge/Librosa-Audio_Analysis-orange)
![Scipy](https://img.shields.io/badge/Scipy-Signal_Processing-green)

## 📖 Sobre o Projeto

Este projeto foi desenvolvido para demonstrar a aplicação prática da **Transformada de Fourier (FFT)** e da teoria de **Circuitos Elétricos** no processamento de áudio.

O software permite que o usuário carregue três arquivos de áudio distintos (representando faixas de frequência Grave, Média e Aguda), realiza a mixagem digital desses sinais e aplica um **Filtro Passa-Baixa (Low-Pass)** simulado matematicamente para recuperar o sinal original de baixa frequência.

### Principais Funcionalidades
- **Interface Gráfica (GUI):** Seleção de arquivos interativa usando `tkinter`.
- **Mixagem de Áudio:** Combinação de sinais no domínio do tempo.
- **Análise Espectral:** Visualização das frequências usando a Transformada Rápida de Fourier (FFT).
- **Simulação de Circuito RC:** Implementação digital da função de transferência de um filtro analógico de 1ª ordem.
- **Comparação Visual:** Gráficos detalhados comparando o sinal misturado, o sinal filtrado e o sinal alvo original.

## 🛠️ Tecnologias Utilizadas

- **Python 3**: Linguagem base.
- **NumPy**: Manipulação de arrays e cálculos matemáticos.
- **Matplotlib**: Plotagem dos gráficos (Tempo e Frequência).
- **Librosa**: Carregamento e pré-processamento de áudio (conversão mono/resample).
- **SciPy (fft)**: Algoritmos de Transformada de Fourier.
- **Tkinter**: Interface para seleção de arquivos.

## ⚡ Fundamentação Teórica

O núcleo do projeto baseia-se na função de transferência de um circuito RC série (Resistor-Capacitor), onde a saída é tomada sobre o capacitor.

A frequência de corte ($f_c$) é definida por:
$$f_c = \frac{1}{2\pi RC}$$

A filtragem é realizada no domínio da frequência multiplicando o espectro do sinal de entrada $X(j\omega)$ pela função de transferência do filtro $H(j\omega)$:

$$H(j\omega) = \frac{1}{1 + j\omega RC}$$

Onde $\omega$ é a frequência angular ($2\pi f$).

## 🚀 Como Executar

### Pré-requisitos
Certifique-se de ter o Python instalado. Em seguida, instale as dependências:

```bash
pip install numpy matplotlib librosa scipy
```
### Como clonar o repositorio
```
git clone [https://github.com/SEU-USUARIO/NOME-DO-REPO.git](https://github.com/SEU-USUARIO/NOME-DO-REPO.git)
```
### Como execultar o projeto
```
python main.py
```
