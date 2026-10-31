class Carro:
    def __init__(self, marca, modelo, ano):
        self.marca = marca
        self.modelo = modelo
        self.ano = ano
        self.ligado = False
        self.velocidade = 0

    def ligar(self):
        self.ligado = True
        print(f"O {self.marca} {self.modelo} ({self.ano}) ligou. VRUUUUUUUUMMMMMMMMMMMMMMMMMMMMM")

    def acelerar(self, incremento):
        if self.ligado:
            self.velocidade += incremento
            print(f"O {self.modelo} acelerou para {self.velocidade} km/h.")
        else:
            print(f"Não dá para ligar! O {self.modelo} bufo.")

#meus carrinhos
carro1 = Carro("McLaren", "McLaren P1", 2023)
carro2 = Carro("Volkswagen", "Fuscão", 1935)


print("--- CARRO 1 ---")
carro1.ligar()
carro1.acelerar(60)

print("\n--- CARRO 2 ---")

carro2.acelerar(40)
