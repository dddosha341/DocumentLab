# Any Dll Reflection

В данной программе подгружается любая DLL однокурсника. Взаимодействие с объектами происходит через System.Reflection (динамическое взаимодействие)

# Как работать с этим?

Ваш класс контейнер должен реализовывать интерфейс IVelosiped с методами:

```
public interface IVelosiped
{
  public void SortInt();
  public void SortString();
  public void Randomize();
  public string[] Print();
}
```

Сортировки вы настраиваете сами в своём классе-контейнере.

Вывод печати идёт через массив, чтобы затем вы смогли это привязать к форме. 

Можете использовать этот шаблон.
