import random
import datetime

tasks = []  # Struktur data list untuk menyimpan tugas

def add_task(task_name, priority):
    task = {
        "id": random.randint(1000, 9999),  # ID unik untuk setiap tugas
        "name": task_name,
        "priority": priority,
        "created_at": datetime.datetime.now().strftime("%Y-%m-%d %H:%M:%S")
    }
    tasks.append(task)
    print(f"Tugas '{task_name}' telah ditambahkan!\n")

def view_tasks():
    if not tasks:
        print("Tidak ada tugas yang tersedia.\n")
        return
    print("Daftar Tugas:")
    for task in tasks:
        print(f"ID: {task['id']} | Nama: {task['name']} | Prioritas: {task['priority']} | Dibuat: {task['created_at']}")
    print()

def remove_task(task_id):
    global tasks
    tasks = [task for task in tasks if task["id"] != task_id]
    print(f"Tugas dengan ID {task_id} telah dihapus!\n")

while True:
    print("Sistem Manajemen Tugas")
    print("1. Tambah Tugas")
    print("2. Lihat Tugas")
    print("3. Hapus Tugas")
    print("4. Keluar")
    
    choice = input("Pilih menu: ")
    if choice == "1":
        name = input("Masukkan nama tugas: ")
        priority = input("Masukkan prioritas (Tinggi/Sedang/Rendah): ")
        add_task(name, priority)
    elif choice == "2":
        view_tasks()
    elif choice == "3":
        task_id = int(input("Masukkan ID tugas yang ingin dihapus: "))
        remove_task(task_id)
    elif choice == "4":
        print("Keluar dari program.")
        break
    else:
        print("Pilihan tidak valid. Coba lagi.\n")
