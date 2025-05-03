# chess-game  
def init_board():
    board = [["." for _ in range(8)] for _ in range(8)]
    board[7][4] = "PK"  # Player King
    board[7][0] = "PR"  # Player Rook
    board[0][4] = "CK"  # Computer King
    board[0][7] = "CR"  # Computer Rook
    return board

def print_board(board):
    print("  A B C D E F G H")
    for i, row in enumerate(board):
        print(f"{8 - i} " + " ".join(row))
    print()
