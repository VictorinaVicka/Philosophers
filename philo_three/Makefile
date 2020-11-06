# **************************************************************************** #
#                                                                              #
#                                                         :::      ::::::::    #
#    Makefile                                           :+:      :+:    :+:    #
#                                                     +:+ +:+         +:+      #
#    By: tfarenga <tfarenga@student.42.fr>          +#+  +:+       +#+         #
#                                                 +#+#+#+#+#+   +#+            #
#    Created: 2020/11/02 14:02:00 by tfarenga          #+#    #+#              #
#    Updated: 2020/11/06 16:46:05 by tfarenga         ###   ########.fr        #
#                                                                              #
# **************************************************************************** #

NAME = philo_three

CC = clang
FLAGS = -Wall -Werror -Wextra
LIBS = -lpthread

SRC = philo_three.c other.c other_next.c functions.c init.c sim.c
OBJ = $(SRC:.c=.o)

%.o : %.c
	@$(CC) $(FLAGS) -c $< -o $@

.PHONY: all clean fclean re

all: $(NAME)

$(NAME): $(OBJ)
	@$(CC) $(FLAGS) -I . $(OBJ) -o $(NAME) $(LIBS)

clean:
	@rm -f $(OBJ)

fclean: clean
	@rm -f $(NAME)

re: fclean all