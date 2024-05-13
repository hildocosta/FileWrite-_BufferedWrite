<p align="center">
  <img src="https://github.com/hildocosta/hildocosta-Curso-Java--Nelio-Alves/blob/main/logo.png" width="300">
</p>
<h1 align="center">🚀 Explorando Escrita de Arquivo Texto em Java</h1>
<p>🔥 Bem-vindo ao repositório dedicado à exploração da escrita de arquivos de texto na linguagem de programação Java. Aqui, você encontrará informações e exemplos práticos sobre como usar as classes FileWriter e BufferedWriter para escrever e manipular dados de arquivos de texto em seus programas Java.</p>
<p>🎓 Este repositório é voltado para estudantes e desenvolvedores que desejam aprender como escrever dados em arquivos de texto de forma eficiente e prática em Java. Aqui, você encontrará explicações detalhadas, exemplos de código e exercícios para aprimorar suas habilidades de escrita de arquivos.</p>
<p>💡 Ao explorar a escrita de arquivos texto em Java, você aprenderá como abrir, escrever e manipular dados de arquivos de texto usando as classes FileWriter e BufferedWriter. Essas classes fornecem métodos simples e eficazes para trabalhar com arquivos de texto, permitindo que você salve e modifique informações em arquivos de forma fácil e rápida.</p>
<h2 align="center">🔒 Licença</h2>
<p>⚖️ Este projeto está licenciado sob a <a href="LICENSE">Licença MIT</a>.</p>
<h2 align="center">📧 Contato</h2>
<h3>🔗 Redes Sociais e Contato</h3>
<ul>
  <li>📌 GitHub: <a href="https://github.com/hildocosta">hildocosta</a></li>
  <li>💼 LinkedIn: <a href="https://www.linkedin.com/in/hildo-costa-b83812231/">Hildo Costa</a></li>
  <li>✉️ Email: hildo.costa@pm.pr.gov.br</li>
</ul>
<p>Agora que estamos preparados, vamos explorar como escrever arquivos de texto em Java!</p>
<h2 align="center">🚀 Vamos Começar</h2>
<h3>🔥 Escrita de Arquivo Texto em Java</h3>
<p>Para escrever dados em um arquivo de texto em Java, você pode usar as classes FileWriter e BufferedWriter. A classe FileWriter é usada para escrever caracteres em um arquivo, enquanto a classe BufferedWriter é usada para escrever texto em um buffer antes de gravá-lo em um arquivo.</p>
<p>Veja um exemplo de código para escrever em um arquivo de texto em Java usando FileWriter e BufferedWriter:</p>

```java
import java.io.BufferedWriter;
import java.io.FileWriter;
import java.io.IOException;

public class Main {

    public static void main(String[] args) {
        
        // Array contendo as linhas a serem escritas no arquivo
        String[] linhas = new String[] {"Bom dia", "Boa tarde", "Boa noite"};
        
        // Caminho do arquivo de saída
        String caminho = "caminho/do/arquivo.txt";
        
        try (BufferedWriter bw = new BufferedWriter(new FileWriter(caminho))) {
            // Abrindo o arquivo para escrita e criando um BufferedWriter usando o try-with-resources
            
            // Escrevendo cada linha do array no arquivo
            for (String linha : linhas) {
                bw.write(linha); // Escreve a linha no arquivo
                bw.newLine(); // Escreve uma nova linha após cada linha do texto
            }
        } catch (IOException e) { // Captura possíveis exceções de E/S (IOException)
            e.printStackTrace(); // Imprime a pilha de erros
        }
            
    }

}

```

<p>Este código escreve as strings contidas no array `linhas` em um arquivo de texto. Ele utiliza o BufferedWriter e FileWriter para escrever eficientemente no arquivo especificado. O bloco try-with-resources garante que os recursos sejam fechados automaticamente após o uso. Se ocorrer uma exceção de E/S durante a escrita no arquivo, a pilha de erros será impressa.</p>


<p>Agora que você entende como escrever arquivos de texto em Java usando FileWriter e BufferedWriter, experimente criar e manipular seus próprios arquivos para praticar e aprimorar suas habilidades!</p>
