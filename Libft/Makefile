# **************************************************************************** #
#                                                                              #
#                                                         :::      ::::::::    #
#    Makefile                                           :+:      :+:    :+:    #
#                                                     +:+ +:+         +:+      #
#    By: nanasser <nanasser@student.42.fr>          +#+  +:+       +#+         #
#                                                 +#+#+#+#+#+   +#+            #
#    Created: 2025/01/17 21:00:03 by nanasser          #+#    #+#              #
#    Updated: 2025/01/27 19:38:00 by nanasser         ###   ########.fr        #
#                                                                              #
# **************************************************************************** #

SRC = ./ft_atoi.c \
./ft_bzero.c \
./ft_calloc.c \
./ft_isalnum.c \
./ft_isalpha.c \
./ft_isascii.c \
./ft_isdigit.c \
./ft_isprint.c \
./ft_memchr.c \
./ft_memcmp.c \
./ft_memcpy.c \
./ft_memmove.c \
./ft_memset.c \
./ft_strchr.c \
./ft_strdup.c \
./ft_strlcat.c \
./ft_strlcpy.c \
./ft_strlen.c \
./ft_strncmp.c \
./ft_strnstr.c \
./ft_strrchr.c \
./ft_tolower.c \
./ft_toupper.c \
./ft_substr.c \
./ft_strjoin.c \
./ft_strtrim.c \
./ft_split.c \
./ft_itoa.c \
./ft_strmapi.c \
./ft_striteri.c \
./ft_putchar_fd.c \
./ft_putstr_fd.c \
./ft_putendl_fd.c \
./ft_putnbr_fd.c \

BONUS_SRC = ./ft_lstnew.c \
./ft_lstadd_front.c \
./ft_lstsize.c \
./ft_lstlast.c \
./ft_lstadd_back.c \
./ft_lstdelone.c \
./ft_lstclear.c \
./ft_lstiter.c \
./ft_lstmap.c \

OBJ = $(SRC:.c=.o)

BONUS_OBJ = $(BONUS_SRC:.c=.o)

CC		= cc

CFLAGS += -Wall -Werror -Wextra

NAME = libft.a

all:$(NAME)

$(NAME)	:	$(OBJ)
	ar -rcs $(NAME) $(OBJ)

%.o : %.c
	$(CC) $(CFLAGS) -c $< -o $@

bonus: $(OBJ) $(BONUS_OBJ)
	ar -rcs $(NAME) $(OBJ) $(BONUS_OBJ)

clean:
	rm -f $(OBJ) $(BONUS_OBJ)

fclean: clean
	rm -f $(NAME)

re: fclean $(NAME)

.PHONY: all clean fclean re