import random
import copy

class macaron:
    def __init__(self, color):
        self.color = color  # 1 for black, -1 for white
    
    def get_move(self, board):
        valid_moves = self.get_valid_moves(board)
        return random.choice(valid_moves) if valid_moves else None

    def get_valid_moves(self, board):
        valid_moves = []
        for row in range(8):
            for col in range(8):
                if self.is_valid_move(board, row, col):
                    valid_moves.append((row, col))
        return valid_moves

    def is_valid_move(self, board, row, col):
        if board[row][col] != 0:
            return False
        return True 
