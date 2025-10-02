## PROJETO HAL - DRIVER DE TEMPERATURA


🎯 Objetivo

Criar driver Zephyr para sensor AT30TSE752A na placa SAM D21.

🛠️ Ferramentas Instaladas

Zephyr RTOS

West build system

Renode (emulador)

Zephyr SDK

✅ Testes Realizados

✅ Compilação QEMU - "Hello World" funcionando

✅ Compilação SAMD21 - Binário gerado com sucesso

✅ Renode + Zephyr - Integração testada 


💻 Comandos Principais

# Ativar ambiente
cd ~/zephyrproject/zephyr && source zephyr-env.sh

# Compilar  
west build -b samd21_xpro meu_projeto

# Testar
west build -b qemu_cortex_m3 samples/hello_world && west build -t run
