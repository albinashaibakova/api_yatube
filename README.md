# api_yatube

<h1> api_yatube </h1>

<h3> О проекте: </h3>
<p> API_YATUBE - API для сервиса YATUBE </p>

<p> API доступен только аутентифицированным пользователям.
Аутентифицированный пользователь авторизован на изменение и удаление своего контента;
в остальных случаях доступ предоставляется только для чтения.
При попытке изменить чужие данные должен возвращаться код ответа 403 Forbidden.
</p>

<h3> Эндпоинты API: </h3>
<p>
<li> api/v1/api-token-auth/ (POST): передаём логин и пароль, получаем токен. </li>
<li> api/v1/posts/ (GET, POST): получаем список всех постов или создаём новый пост. </li>
<li> api/v1/posts/{post_id}/ (GET, PUT, PATCH, DELETE): получаем, редактируем или удаляем пост с идентификатором{post_id}. </li>
<li> api/v1/groups/ (GET): получаем список всех групп. </li>
<li> api/v1/groups/{group_id}/ (GET): получаем информацию о группе с идентификатором {group_id}. </li>
<li> api/v1/posts/{post_id}/comments/ <br>
(GET): получаем список всех комментариев поста с идентификатором post_id <br>
(POST): создаём новый комментарий для поста с идентификатором {post_id}. </li>
<li> api/v1/posts/{post_id}/comments/{comment_id}/ (GET, PUT, PATCH, DELETE): получаем, редактируем или удаляем комментарий с идентификатором {comment_id} в посте с id=post_id. </li>
</p>
<p> Для запуска проекта: <br>
создайте виртуальное окружение и установите зависимости из файла <i> requirements.txt </i>
</p>
<code>
python -m venv venv
</code>
<br>
<code>
pip install -r requirements.txt
</code>
<p> Запустите проект <br>
<code>
python manage.py runserver
</code>
</p> 
<p>
Для тестирования API сервиса воспользуйтесь коллекцией Postman <i>[postman_collection]</i>
</p>



<p> <h3> Авторы </h3> 
Альбина Шайбакова - Backend Developer
</p>