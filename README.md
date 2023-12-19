# Pratica-_6_Embarcados

Ricardo Dias 12704331
Gustavo Rinaldi 10845022

# Controle de acesso via Tag RFID:

Nesta atividade foi montado um circuito com um módulo RF conectado a uma Raspberry para verificar, por meio do código “validacaoRFID.py”, se o cartão, que funciona como tag RFID, tem sua ID cadastrada no código. Se for a cadastrada, é informada uma mensagem via terminal dizendo “acesso liberado” e um led verde pisca. Se não for a cadastrada, é informada uma mensagem via terminal dizendo “acesso negado” e um led vermelho pisca.

O novo conceito apresentado nessa prática é o uso da biblioteca “mfrc522”  que fornece a classe “SimpleMFRC522” para criar o objeto “leitor” para o módulo RF realizar e informar a leitura do ID das tags  para o código fazer a comparação com a ID já salva.

Nas imagens 1, 2 e 3 é possível verificar a montagem da prática bem como seu funcionamento para os casos em que o código espera alguma tag se aproximar do leitor físico via RF, a leitura de uma tag cadastrada e a leitura de uma tag não cadastrada, respectivamente.

![WhatsApp Image 2023-12-18 at 16 10 34](https://github.com/Ricas78/Pratica-_6_Embarcados/assets/145056468/a4a80829-c2d3-40cf-9239-6b057c734c26)
Imagem 1 - Sistema embarcado esperando a aproximação de uma tag.

![WhatsApp Image 2023-12-18 at 16 11 40](https://github.com/Ricas78/Pratica-_6_Embarcados/assets/145056468/ee25ef23-0f8b-4360-8e5f-0d3769f8e2ae)
Imagem 2 - Sistema embarcado após uma tag cadastrada ser lida.

![WhatsApp Image 2023-12-18 at 16 13 06](https://github.com/Ricas78/Pratica-_6_Embarcados/assets/145056468/c8321446-f703-43d1-8a82-e214457dd8f1)
Imagem 3 - Sistema embarcado após uma tag não cadastrada ser lida.

# Detecção facial via câmera:

Nesta atividade foi montado um circuito com um módulo de câmera conectado a uma Raspberry para detecção facial, por meio do código “CAM2.py”, onde ao ser executado abre a câmera e se um rosto é detectado, é tirada uma foto só do quadrado de identificação do rosto na imagem (salva na mesma pasta local em que o código se encontra) que é sinalizada por uma mensagem via terminal dizendo “Rosto reconhecido” e um led piscando.  

O novo conceito apresentado nessa prática é o uso das bibliotecas cv2 (OpenCV) e picamera2 para, respectivamente, fornecer modelos pré-treinados para detecção de faces e o uso da câmera da Raspberry Pi. Além disso, foi usado o arquivo “haarcascade_frontalface_default.xml” como algoritmo inteligente que aplica um método de classificação de imagens para detecção facial.

Na imagem 4 é possível verificar a montagem da prática bem como seu funcionamento ao ser detectado um rosto na imagem da câmera.

![WhatsApp Image 2023-12-18 at 15 33 28](https://github.com/Ricas78/Pratica-_6_Embarcados/assets/145056468/405fda8f-2dd7-4470-9d45-e52da1d6711d)
Imagem 4 - Sistema embarcado após reconhecer um rosto.
