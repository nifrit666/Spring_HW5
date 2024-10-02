## Фреймворк Spring (семинары)
## Урок 5. Spring Data для работы с базами данных
## Задание: Используйте Spring Data для создания репозитория, которое взаимодействует с базой данных. Создайте CRUD операции для класса Person.

/*
Вам предстоит создать приложение для управления списком задач с использованием Spring Boot и Spring Data JPA.
Требуется реализовать следующие функции:

Добавление задачи. Подсказка метод в контроллере: @PostMapping public Task addTask(@RequestBody Task task)
Просмотр всех задач. Подсказка метод в контроллере: @GetMapping public List<Task> getAllTasks()
Просмотр задач по статусу (например, "завершена", "в процессе", "не начата"). Подсказка метод в контроллере:
@GetMapping("/status/{status}") public List<Task> getTasksByStatus(@PathVariable TaskStatus status)
Изменение статуса задачи. Подсказка метод в контроллере: @PutMapping("/{id}")
public Task updateTaskStatus(@PathVariable Long id, @RequestBody Task task)
Удаление задачи.
Подсказка метод в контроллере: @DeleteMapping("/{id}")
public void deleteTask(@PathVariable Long id)

Репозитроий подсказка public interface TaskRepository extends JpaRepository<Task, Long>

*/