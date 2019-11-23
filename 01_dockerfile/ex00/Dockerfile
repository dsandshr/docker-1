# **************************************************************************** #
#                                                                              #
#                                                         :::      ::::::::    #
#    Dockerfile                                         :+:      :+:    :+:    #
#                                                     +:+ +:+         +:+      #
#    By: dsandshr <dsandshr@student.42.fr>          +#+  +:+       +#+         #
#                                                 +#+#+#+#+#+   +#+            #
#    Created: 2019/09/22 21:08:16 by dsandshr          #+#    #+#              #
#    Updated: 2019/09/22 23:10:41 by dsandshr         ###   ########.fr        #
#                                                                              #
# **************************************************************************** #

FROM alpine

RUN apk	update && \
	apk upgrade && \
	apk add vim

ENTRYPOINT vim
# docker build -t ex00 . - Чтоб построить
# docker run --rm -ti ex00 - Чтоб запустить