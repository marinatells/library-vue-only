<template>
    <div class="container mt-5">
        <h1>Список книг нашей библиотеки</h1>
        <table class="table">
            <thead>
                <tr>
                    <th scope="col">#</th>
                    <th scope="col">Название</th>
                    <th scope="col">Автор</th>
                    <th scope="col">Наличие</th>
                    <th scope="col">Действия</th>
                </tr>
            </thead>
            <tbody>
                <tr>
                    <th scope="row">1</th>
                    <td>Война и мир</td>
                    <td>Л. Н. Толстой</td>
                    <td>
                        <button type="button" class="btn btn-outline-primary" v-on:click="">
                            Доступна
                        </button>
                    </td>
                    <td>
                        <button type="button" class="btn btn-outline-danger" v-on:click="">
                            Удалить
                        </button>
                    </td>
                </tr>

                <!-- Строка с полями для добавления новой книги -->
                <tr>
                    <th scope="row">Добавить</th>
                    <td><input type="text" class="form-control"></td>
                    <td><input type="text" class="form-control"></td>
                    <td></td>
                    <td>
                        <button type="button" class="btn btn-outline-success" v-on:click="">
                            Добавить
                        </button>
                    </td>
                </tr>
            </tbody>
        </table>
    </div>
</template>

<script>
    export default {
        mounted() {
            // Сразу после загрузки страницы подгружаем список книг и отображаем его
            this.loadBookList();
        },
        methods: {
            loadBookList(){

            },
            addBook(){

            },
            deleteBook(id){

            },
            changeBookAvailability(id){

            }
        }
    }
</script>


<style>
    .app {
        background-color: rgb(235, 233, 233);
        padding: 20px;
        text-align: center;
        border-radius: 8px;
    }

    .app nav {
        display: flex;
        justify-content: center;
        gap: 20px;
    }
</style>
