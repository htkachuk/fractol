# **************************************************************************** #
#                                                                              #
#                                                         :::      ::::::::    #
#    Makefile                                           :+:      :+:    :+:    #
#                                                     +:+ +:+         +:+      #
#    By: htkachuk <marvin@42.fr>                    +#+  +:+       +#+         #
#                                                 +#+#+#+#+#+   +#+            #
#    Created: 2017/11/04 15:24:31 by htkachuk          #+#    #+#              #
#    Updated: 2017/11/04 15:24:34 by htkachuk         ###   ########.fr        #
#                                                                              #
# **************************************************************************** #

NAME = libft.a

SRC = ft_strsortwane.c ft_strsortgrow.c ft_sort_wane.c ft_sort_grow.c ft_lstmap.c ft_lstiter.c ft_lstadd.c ft_lstdelone.c ft_lstdel.c ft_putnbr.c ft_lstnew.c ft_putnbr_fd.c ft_itoa.c ft_strsplit.c ft_putstr.c ft_putendl.c ft_putchar_fd.c ft_putstr_fd.c ft_putendl_fd.c ft_putchar.c ft_strtrim.c ft_strjoin.c ft_strsub.c ft_strnequ.c ft_strequ.c ft_strmapi.c ft_strmap.c ft_striteri.c ft_striter.c ft_strdel.c ft_strclr.c ft_strnew.c ft_memdel.c ft_bzero.c ft_isalnum.c ft_isalpha.c ft_isascii.c ft_isdigit.c ft_isprint.c ft_memccpy.c ft_memchr.c ft_memcmp.c ft_memcpy.c ft_memmove.c ft_memset.c ft_strcat.c ft_strchr.c ft_strcmp.c ft_strcpy.c ft_strdup.c ft_strlcat.c ft_strlen.c ft_strncat.c ft_strncmp.c ft_strncpy.c ft_strnstr.c ft_strrchr.c ft_strstr.c ft_tolower.c ft_toupper.c ft_atoi.c ft_memalloc.c

INC = libft.h 

OBJ = $(SRC:.c=.o)

CC = gcc

KEYS = -Wall -Werror -Wextra -c

LIB = ar rc

all: $(NAME)

$(NAME): $(OBJ)
	@ $(LIB) $(NAME) $(OBJ)
	@ ranlib $(NAME)

%.o: %.c $(INC)
	@ gcc -c $(KEYS) -o $@ -c $< -I $(INC)

clean:
	@ /bin/rm -f $(OBJ)

fclean: clean
	@ /bin/rm -f $(NAME)

re: fclean all

.PHONY: re all clean fclean