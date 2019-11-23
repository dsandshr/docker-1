# **************************************************************************** #
#                                                                              #
#                                                         :::      ::::::::    #
#    Dockerfile                                         :+:      :+:    :+:    #
#                                                     +:+ +:+         +:+      #
#    By: dsandshr <dsandshr@student.42.fr>          +#+  +:+       +#+         #
#                                                 +#+#+#+#+#+   +#+            #
#    Created: 2019/09/23 18:19:43 by dsandshr          #+#    #+#              #
#    Updated: 2019/09/25 15:26:19 by dsandshr         ###   ########.fr        #
#                                                                              #
# **************************************************************************** #

FROM ruby

RUN apt-get update && \
	apt-get install -y build-essential libpq-dev nodejs sqlite3

ONBUILD EXPOSE 3000

ONBUILD COPY app /opt/app

ONBUILD WORKDIR /opt/app

ONBUILD RUN bundle install
ONBUILD RUN rake db:migrate
ONBUILD RUN rake db:seed

# docker build -t ft-rails:on-build . - чтоб построить