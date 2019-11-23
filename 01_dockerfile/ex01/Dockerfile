# **************************************************************************** #
#                                                                              #
#                                                         :::      ::::::::    #
#    Dockerfile                                         :+:      :+:    :+:    #
#                                                     +:+ +:+         +:+      #
#    By: dsandshr <dsandshr@student.42.fr>          +#+  +:+       +#+         #
#                                                 +#+#+#+#+#+   +#+            #
#    Created: 2019/09/22 21:30:08 by dsandshr          #+#    #+#              #
#    Updated: 2019/09/23 17:51:07 by dsandshr         ###   ########.fr        #
#                                                                              #
# **************************************************************************** #

FROM debian

ENV TS3SERVER_LICENSE=accept

WORKDIR /home/ts

EXPOSE 9987/udp 10011 30033

RUN apt-get update && \
    apt-get upgrade -y && \
    apt-get install -y bzip2 wget && \
    wget https://files.teamspeak-services.com/releases/server/3.9.1/teamspeak3-server_linux_amd64-3.9.1.tar.bz2 && \
    tar -xvf teamspeak3-server_linux_amd64-3.9.1.tar.bz2

WORKDIR /home/ts/teamspeak3-server_linux_amd64

ENTRYPOINT sh ts3server_minimal_runscript.sh
# docker build -t ex01 . - Чтоб простроить
# docker run --rm -p 9987:9987/udp -p 10011:10011 -p 30033:30033 ex01 - Чтоб запустить