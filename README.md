 Title="MainWindow" Height="720" Width="1280"
        WindowState="Maximized">
    <Grid>
        <Frame x:Name="MainFrame"/>
    </Grid>            

MainFrame.Navigate(new AuthorizationPage());
            MainFrame.NavigationUIVisibility = NavigationUIVisibility.Hidden;



private int currentPage = 0;
private int itemsPerPage = 20;

private void UpdateListView()
{
    myListView.ItemsSource = YourDataList.Skip(currentPage * itemsPerPage).Take(itemsPerPage).ToList();
}

private void LeftButton_Click(object sender, RoutedEventArgs e)
{
    if (currentPage > 0)
    {
        currentPage--;
        UpdateListView();
    }
}

private void RightButton_Click(object sender, RoutedEventArgs e)
{
    if ((currentPage + 1) * itemsPerPage < YourDataList.Count)
    {
        currentPage++;
        UpdateListView();
    } 


<ListView Margin="0,100,0,0" ScrollViewer.HorizontalScrollBarVisibility="Disabled" ScrollViewer.CanContentScroll="False" Grid.Row="1" HorizontalAlignment="Center" x:Name="ProductList" BorderBrush="#FEF9EF" Background="#001242" ScrollViewer.VerticalScrollBarVisibility="Visible" 
                  d:ItemsSource="{d:SampleData ItemCount=3}" Width="1260">
            <ListView.ItemTemplate>
                <DataTemplate>
<StackPanel/>
</DataTemplate>
</ListView.ItemTemplate>
</Listview>

Техническое задание
1 ВВЕДЕНИЕ
1.1 Наименование продукта
Наименование продукта: 
1.2 Назначение и область применения
Продукт предназначен для сотрудников компании, которая занимается ремонтом бытовой техники
2 ТРЕБОВАНИЯ К ПРОГРАММЕ 
2.1 Общие требования
Разработать приложение для компании, занимающейся ремонтом бытовой техники.
По мимо этого, разработать элементы пользовательского интерфейса. 
Интерфейс должен быть интуитивно понятен, а навигация работала корректно.
2.2 Требования к визуальной части
В программном продукте должен применяться и поддерживаться единый стиль. Шрифты должны быть читабельными.
2.3 Требования к функциям приложения
Приложение должно поддерживать одновременное подключение нескольких пользователей, отображение данных в реальном времени и быть стабильным.
	Сотрудник должен иметь возможность просматривать свои данные, такие как баланс и иметь возможность взаимодействовать с ним.
Для директора необходимо будет реализовать функции отчетов для того, чтобы он смог отследить данные, связанные с сотрудниками.
 Также для директора должен быть реализован функционал обновления данных о заработке за единицу товара для сотрудников
3 УСЛОВИЯ ЭКСПЛУАТАЦИИ
Для стабильного функционирования, устанавливаются необходимые минимальные характеристики для смартфона:
− Windows версии 10 и более (не меньше);
− оперативная память 8 Гб и более (не меньше);
− видеокарта с 4 Гб видеопамяти и более (не меньше);
− процессор с частотой 2,8 Ггц и более (не меньше).
4 ТРЕБОВАНИЯ К ПРОГРАММНОЙ ДОКУМЕНТАЦИИ
Состав программной документации включает:
− Техническое задание;
− Руководство системного программиста.
5 СТАДИИ И ЭТАПЫ РАЗРАБОТКИ
Стадии разработки программного приложения:
− анализ требований и разработка технического задания;
− проектирование;
− кодирование;
− тестирование и отладка.
