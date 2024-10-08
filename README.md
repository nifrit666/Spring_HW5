# Фреймворк Spring 

## Урок 5. Spring Data для работы с базами данных

***Задание:***  Используйте **Spring Data** для создания репозитория, которое взаимодействует с базой данных. 

Создайте **CRUD** операции для класса **Person.**


Были реализованны следующие функции:

- Добавление задачи. Метод в контроллере: **@PostMapping public Task addTask(@RequestBody Task task)**
- Просмотр всех задач. Метод в контроллере: **@GetMapping public List<Task> getAllTasks()**
- Просмотр задач по статусу (например, "завершена", "в процессе", "не начата"). Метод в контроллере:
**@GetMapping("/status/{status}") public List<Task> getTasksByStatus(@PathVariable TaskStatus status)**
- Изменение статуса задачи. Метод в контроллере: **@PutMapping("/{id}")
public Task updateTaskStatus(@PathVariable Long id, @RequestBody Task task)**
- Удаление задачи. Метод в контроллере: **@DeleteMapping("/{id}")
public void deleteTask(@PathVariable Long id)**
- Репозитроий. **public interface TaskRepository extends JpaRepository<Task, Long>**
