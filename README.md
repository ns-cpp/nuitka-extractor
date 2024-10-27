# Nuitka Extractor

Nuitka extractor, nuitka derlenmiş Python yürütülebilir dosyalarını ayıklamak için bir araçtır. Özellikle sadece onefile (tek dosya) yürütülebilir dosyalar desteklenir. Araç hem Windows PE hem de Linux ELF ikili dosyalarını çıkarabilir.

Nuitka Python kodunu yerel koda derler. Nuitka ile derlenmiş bir yürütülebilir dosya pyc dosyası içermez. Dolayısıyla bu araç yalnızca DLL'leri, paylaşılan kütüphaneleri ve yürütülebilir dosyaya gömülü diğer ikili varlıkları ayıklayabilir.

## Kullanım

Önceden derlenmiş ikili dosyalar sürümlerden indirilebilir.

Dosyanın yolunu bir argüman olarak geçmeniz yeterlidir.

```
$ ./nuitka-extractor <file name>
```

```
X:\> nuitka-extractor.exe <file name>
```

## ToDo

- İmzalı PE çalıştırılabilirleri henüz desteklenmemektedir. Çıkarma işleminden önce sertifikayı silin.
- Sabit kodlanmış bir çıkarma dizinine sahip yürütülebilir dosyalar için destek. Bu tür yürütülebilir dosyalar için, nuitka her gömülü dosyanın crc32'sini yüke dahil eder. Böylece yük formatı biraz değişir.

## License

Nuitka extractor is released under the MIT license.
