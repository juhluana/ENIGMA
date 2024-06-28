# ENIGMA
ENIGMA
input('digite seu código')

substituicoes = {
  '6': 'F',
  '5': 'E',
  '50': 'L',
  '1': 'I',
  '26': 'Z',
  'MM': '2000',
  'R': '18'
}

mensagem_codificada = "6550126MMR"

mensagem_decodificada = ["FELIZ 2018"]

sequencia = ''


for caractere in mensagem_codificada:
  sequencia += caractere  

  if sequencia in substituicoes:
      mensagem_decodificada.append(substituicoes[sequencia])
      

mensagem_decodificada = ''.join(mensagem_decodificada)

print(f"Mensagem codificada: {mensagem_codificada}")
print(f"Mensagem decodificada {''.join(mensagem_decodificada)}")

