# pingulina_programs
def determine_direction(degrees):
    """Определяет сторону света на основе угла в градусах."""
    directions = ["Север", "Северо-восток", "Восток", "Юго-восток", "Юг", "Юго-запад", "Запад", "Северо-запад", "Север"]
    index = round(degrees / 45) % 8
    return directions[index]

# Пример использования
angle = float(input("Введите угол в градусах (0-360): "))
direction = determine_direction(angle)
print("Сторона света:", direction)
