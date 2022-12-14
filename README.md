# Chips Widget :
```
Semantics(
  label: 'Dietary preference chips',
  child: Wrap(
    spacing: 5.0,
    children: [
      Chip(label: 'Vegan'),
      Chip(label: 'Vegetarian'),
      Chip(label: 'Gluten-free'),
      Chip(label: 'Dairy-free'),
      Chip(label: 'Paleo')
    ],
  ),
)
```
```
Semantics(
  label: 'Chip Widget',
  child: Chip(
    label: 'Label',
    avatar: CircleAvatar(
      child: Text('A'),
    ),
  ),
)
```
```
Semantics(
  label: "Chip Widget",
  child: Chip(
    label: Text("Chip Label"),
  ),
);
```
```
Semantics(
  label: 'Chips widget',
  child: Chips(
    label: 'Chips',
    avatar: Icon(Icons.face),
    onDeleted: () {},
  ),
);
```

# Floating Action Button (FAB) :
```
Semantics(
  label: 'FAB Widget',
  button: true,
  child: FloatingActionButton(
    onPressed: () {},
    child: Icon(Icons.add),
  ),
)
```
```
Semantics(
  label: 'FAB widget',
  child: FloatingActionButton(
    child: Icon(Icons.add),
    onPressed: () {},
  ),
);
```
```
Semantics(
  label: 'Tambah item',
  hint: 'Tekan untuk menambahkan item ke dalam daftar',
  button: true,
  child: FloatingActionButton(
    onPressed: () {},
    child: Icon(Icons.add),
  ),
);
```
```
Semantics(
  label: "Floating Action Button",
  button: true,
  child: FloatingActionButton(
    onPressed: () {},
    child: Icon(Icons.add),
  ),
);
```

# Textbox Widget
```
Semantics(
  label: 'Textbox Widget',
  textField: true,
  child: TextField(
    decoration: InputDecoration(
      labelText: 'Enter text here',
    ),
  ),
)
```
```
Semantics(
  label: 'Nama',
  hint: 'Masukkan nama Anda',
  child: TextField(
    decoration: InputDecoration(
      labelText: 'Nama',
    ),
  ),
);
```
```
Semantics(
  label: 'Masukkan nama',
  hint: 'Tekan untuk mengaktifkan input teks',
  textField: true,
  child: TextField(
    decoration: InputDecoration(
      labelText: 'Nama',
    ),
  ),
);
```
```
Semantics(
  child: TextField(
    decoration: InputDecoration(
      labelText: "Nama",
      hintText: "Masukkan nama Anda",
    ),
  ),
  label: "Input nama",
  hint: "Untuk memasukkan nama Anda",
);
```
```
Semantics(
  label: "Text Box",
  textField: true,
  child: TextField(
    decoration: InputDecoration(
      labelText: "Enter some text",
    ),
  ),
);
```
```
Semantics(
  label: 'Textbox widget',
  child: TextField(
    decoration: InputDecoration(
      labelText: 'Enter text here',
    ),
  ),
);
```

# Radio Button Widget
```
Semantics(
  label: 'Radio Button Widget',
  radio: true,
  child: Radio(
    value: 0,
    groupValue: 0,
    onChanged: (val) {},
  ),
)
```
```
Semantics(
  label: 'Jenis kelamin',
  child: Row(
    children: [
      Radio(
        value: 'Laki-laki',
        groupValue: _jenisKelamin,
        onChanged: (value) => setState(() => _jenisKelamin = value),
      ),
      Text('Laki-laki'),
    ],
  ),
);
```
```
Semantics(
  label: 'Pilih jenis kelamin',
  hint: 'Tekan untuk memilih jenis kelamin',
  radio: true,
  child: Radio(
    value: 'Laki-laki',
    groupValue: _jenisKelamin,
    onChanged: (String value) {
      setState(() {
        _jenisKelamin = value;
      });
    },
  ),
);
```
```
Semantics(
  child: Radio(
    value: "Pria",
    groupValue: gender,
    onChanged: (value) => setState(() => gender = value),
  ),
  label: "Pria",
  hint: "Pilih jenis kelamin pria",
);
```
```
Semantics(
  label: "Radio Button",
  checked: true,
  child: Radio(
    value: 1,
    groupValue: 1,
    onChanged: (value) {},
  ),
);
```
```
Semantics(
  label: 'Radio button widget',
  child: Radio(
    value: 'radio button 1',
    groupValue: _radioValue,
    onChanged: (value) {
      setState(() {
        _radioValue = value;
      });
    },
  ),
);
```

# Spinner Widget
```
Semantics(
  label: 'Spinner Widget',
  button: true,
  child: DropdownButton(
    items: [
      DropdownMenuItem(
        child: Text('Option 1'),
        value: 1,
      ),
      DropdownMenuItem(
        child: Text('Option 2'),
        value: 2,
      ),
    ],
    onChanged: (val) {},
  ),
)
```
```
Semantics(
  label: 'Pilih negara',
  hint: 'Pilih negara asal Anda',
  child: DropdownButton(
    value: _negara,
    items: _listNegara.map((String value) {
      return DropdownMenuItem(
        value: value,
        child: Text(value),
      );
    }).toList(),
    onChanged: (value) => setState(() => _negara = value),
  ),
);
```
```
Semantics(
  child: DropdownButton(
    items: [
      DropdownMenuItem(
        child: Text("Pilih salah satu"),
        value: null,
      ),
      DropdownMenuItem(
        child: Text("1"),
        value: 1,
      ),
      DropdownMenuItem(
        child: Text("2"),
        value: 2,
      ),
      DropdownMenuItem(
        child: Text("3"),
        value: 3,
      ),
    ],
    onChanged: (value) => setState(() => selectedValue = value),
    value: selectedValue,
  ),
  label: "Pilih angka",
  hint: "Untuk memilih angka",
);
```
```
Semantics(
  label: "Spinner",
  busy: true,
  child: CircularProgressIndicator(),
);
```
```
Semantics(
  label: 'Spinner widget',
  child: SpinKitWave(
    color: Colors.blue,
  ),
);
```
