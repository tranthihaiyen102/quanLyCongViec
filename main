# Phan mem quan ly cong viec

cong_viec = []

while True:
    print("\n----- Menu -----")
    print("1. Thêm công việc")
    print("2. Hiển thị danh sách công việc")
    print("3. Xóa công việc")
    print("4. Tìm kiếm công việc")
    print("5. Thoát")

    lua_chon = input("Chọn chức năng (1/2/3/4/5): ")

    if lua_chon == "1":
        cong_viec_moi = input("Nhập công việc mới: ")
        cong_viec.append(cong_viec_moi)
        print(f"Thêm công việc '{cong_viec_moi}' thành công!")
    elif lua_chon == "2":
        print("\nDanh sách công việc:")
        if not cong_viec:
            print("Không có công việc nào.")
        else:
            for i, cv in enumerate(cong_viec, start=1):
                print(f"{i}. {cv}")
    elif lua_chon == "3":
        print("\nDanh sách công việc:")
        if not cong_viec:
            print("Không có công việc nào để xóa.")
        else:
            for i, cv in enumerate(cong_viec, start=1):
                print(f"{i}. {cv}")
            try:
                idx = int(input("Chọn số công việc muốn xóa: "))
                if 1 <= idx <= len(cong_viec):
                    xoa_cv = cong_viec.pop(idx - 1)
                    print(f"Đã xóa công việc '{xoa_cv}'.")
                else:
                    print("Số công việc không hợp lệ.")
            except ValueError:
                print("Vui lòng nhập một số nguyên.")
    elif lua_chon == "4":
        tu_khoa = input("Nhập từ khóa tìm kiếm: ")
        ket_qua = [cv for cv in cong_viec if tu_khoa.lower() in cv.lower()]
        print("\nKết quả tìm kiếm:")
        if ket_qua:
            for i, cv in enumerate(ket_qua, start=1):
                print(f"{i}. {cv}")
        else:
            print("Không có kết quả nào.")
    elif lua_chon == "5":
        print("Cảm ơn bạn đã sử dụng phần mềm quản lý công việc!")
        break
    else:
        print("Chức năng không hợp lệ. Vui lòng chọn lại.")
