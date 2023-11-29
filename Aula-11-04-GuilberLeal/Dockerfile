FROM kathara/quagga

RUN apt-get update

RUN apt-get install -y isc-dhcp-server

# O openresolv contorna o problema da renomeação do /etc/resolv.conf
# (o docker monta este arquivo e por isso não há como remove-lo ou renomea-lo)
# (não testado ainda!)
RUN apt-get install -y openresolv