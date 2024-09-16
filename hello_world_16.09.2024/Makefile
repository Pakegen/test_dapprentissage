# **************************************************************************** #
#                                                                              #
#                                                         :::      ::::::::    #
#    Makefile                                           :+:      :+:    :+:    #
#                                                     +:+ +:+         +:+      #
#    By: quenalla <quenalla@student.42.fr>          +#+  +:+       +#+         #
#                                                 +#+#+#+#+#+   +#+            #
#    Created: 2024/09/16 13:18:49 by quenalla          #+#    #+#              #
#    Updated: 2024/09/16 14:13:42 by quenalla         ###   ########.fr        #
#                                                                              #
# **************************************************************************** #

CC = gcc

NAME = hello.a

CFLAG = -Wall -Werror -Wextra

SRC =	hello.c\
		main.c\

OBJ = $(SRC:.c=.o)


all: $(NAME)

%.o: %.c
	$(CC) $(CFLAG) -c $< -o $@

$(NAME): $(OBJ)
	ar rcs $(NAME) $(OBJ)

clean:
	rm -f $(OBJ)

fclean: clean
	rm -f $(NAME)

re: fclean all

