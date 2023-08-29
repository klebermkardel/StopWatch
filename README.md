# Aplicativo de Cronômetro em Console

Este é um aplicativo de console que implementa um cronômetro simples, permitindo que os usuários configurem um temporizador regressivo para um intervalo de tempo especificado. O aplicativo exibe a contagem, mostrando os segundos restantes no console, e sinaliza a conclusão da contagem. Os usuários têm a opção de configurar o tempo em segundos ou minutos.

## Como Usar

1. Execute o programa compilando e executando o código C# fornecido no arquivo `Program.cs`.

2. O menu será exibido, solicitando que você insira o tempo desejado para a contagem. Você pode especificar o tempo em segundos ou minutos usando o seguinte formato:
   - S = Segundo => 10s = 10 segundos
   - M = Minuto => 1m = 1 minuto
   - 0 = Sair

3. A contagem começará, exibindo mensagens de "Pronto...", "Preparar...", e "Iniciar..." com intervalos de um segundo entre elas.

4. Assim que a contagem iniciar, o tempo restante será exibido no console, atualizando a cada segundo até que o tempo especificado seja alcançado.

5. Após a conclusão da contagem, o aplicativo exibirá "Cronômetro finalizado" por um breve momento antes de retornar ao menu principal.

6. Para sair do aplicativo, insira "0" quando for solicitado o tempo da contagem.

## Explicação do Código

O código está estruturado da seguinte forma:

- **Método Principal:** Ponto de entrada do aplicativo. Chama o método `Menu` para iniciar a interação com o usuário.

- **Método Menu:** Exibe o menu e obtém a entrada do usuário para determinar o tempo e a unidade da contagem (segundos ou minutos). Se a entrada for "0", o aplicativo é encerrado. Em seguida, ele chama o método `PreStart`.

- **Método PreStart:** Exibe mensagens de "Pronto...", "Preparar...", e "Iniciar..." com intervalos de um segundo usando `Thread.Sleep`. Em seguida, chama o método `Start`.

- **Método Start:** Inicia o loop da contagem, atualizando a exibição do console com o tempo restante a cada segundo até que o tempo da contagem seja alcançado. Após a conclusão, exibe uma mensagem antes de retornar ao menu principal.

## Notas de Uso

- Este é um aplicativo de console básico destinado a fins educacionais e pode ser usado como ponto de partida para aplicativos de cronômetro mais complexos.

- O código pode ser aprimorado adicionando tratamento de erros para a entrada do usuário, permitindo pausar e reiniciar a contagem, ou até mesmo adicionando recursos adicionais como alertas sonoros.

- Esteja ciente de que a precisão da contagem pode ser afetada pelo tempo de processamento do sistema e pelas operações de impressão no console.

Sinta-se à vontade para modificar e estender o código de acordo com suas necessidades ou explorar recursos mais avançados em sua implementação.
