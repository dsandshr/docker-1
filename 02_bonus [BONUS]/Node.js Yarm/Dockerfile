# **************************************************************************** #
#                                                                              #
#                                                         :::      ::::::::    #
#    Dockerfile                                         :+:      :+:    :+:    #
#                                                     +:+ +:+         +:+      #
#    By: dsandshr <dsandshr@student.42.fr>          +#+  +:+       +#+         #
#                                                 +#+#+#+#+#+   +#+            #
#    Created: 2019/09/24 17:30:47 by dsandshr          #+#    #+#              #
#    Updated: 2019/09/24 17:41:15 by dsandshr         ###   ########.fr        #
#                                                                              #
# **************************************************************************** #

FROM alpine

RUN apk update && \
	apk upgrade && \
	apk add yarn

ENTRYPOINT yarn --version

# docker build -t yarn .
# docker run -it --rm yarn