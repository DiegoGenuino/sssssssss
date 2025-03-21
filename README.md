# sssssssss



<!DOCTYPE html>
<html lang="pt-br">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Gerenciador de tarefas</title>
    <link rel="stylesheet" href="style.css">
</head>

<body>
    <section class="section-main">
        <div class="container-main">
            <header class="header-main">
                <div class="logo">🍕 ToDo</div>
                <div><button class="btn-manage-tasks">Gerenciar minhas tarefas</button></div>
            </header>
            <div class="call-to-action">
                <h1>Nunca foi tão <span>tranquilo</span> Gerenciar Tarefas.</h1>
                <div class="action-buttons">
                    <button class="btn-simple-task">Tarefas simplificadas</button>
                    <button class="btn-advanced-task">Tarefas avançadas</button>
                </div>
            </div>
        </div>
    </section>
    <section class="section-tasks">
        <div class="task-creation">
            <h1>Adicione uma tarefa</h1>
            <div class="task-inputs">
                <label for="taskName">Task Name</label>
                <input type="text" name="taskName" id="taskName" placeholder="Enter a task">
                <label for="taskDescription">Task Description</label>
                <input type="text" name="taskDescription" id="taskDescription" placeholder="Enter a description">
                <label for="taskDate">Task Date</label>
                <input type="date" name="taskDate" id="taskDate" placeholder="Enter a task date">
                <label for="taskTime">Task Time</label>
                <input type="time" name="taskTime" id="taskTime" placeholder="Enter a task time">
                <button class="btn-add-task">Adicionar</button>
            </div>
        </div>
        <div class="task-list">
            <h1>Tarefas</h1>
            <div class="task-item">DIEGO</div>
            <div class="task-item">DIEGO</div>
            <div class="task-item">DIEGO</div>
        </div>
    </section>
</body>

</html>



@import url('https://fonts.googleapis.com/css2?family=Poppins:ital,wght@0,100;0,200;0,300;0,400;0,500;0,600;0,700;0,800;0,900;1,100;1,200;1,300;1,400;1,500;1,600;1,700;1,800;1,900&display=swap');

/* Definição das variáveis de cor */
:root {
    --primary-color: #b3eb4d;
    --secondary-color: #ffffff;
    --text-color: #000000;
    --box-shadow-color: rgba(0, 0, 0, 0.61);
}

* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: "Poppins", sans-serif;
}

.section-main {
    width: 100%;
    height: 50vh;
    background-color: var(--primary-color);
    padding: 0 5rem 3rem 5rem;
}

.container-main {
    width: 100%;
    height: 100%;
    padding: 4rem 10rem;
    border-bottom-right-radius: 5rem;
    border-bottom-left-radius: 5rem;
    background: url(assets/container-01-img.svg);
    background-repeat: no-repeat;
    background-size: cover;
    background-position: 100% 5%;
    display: flex;
    flex-direction: column;
    justify-content: space-between;
    gap: 3rem;
    border: solid .1rem var(--secondary-color);
}

.header-main {
    width: 100%;
    height: 5rem;
    display: flex;
    justify-content: space-between;
    align-items: center;
    border: solid 1rem var(--text-color);
    margin: 0 auto;
    background-color: transparent;
    border-radius: 10rem;
    padding: 2rem;
    border: .1rem solid var(--text-color);
}

.logo {
    font-weight: 500;
    font-size: 1.5rem;
}

.call-to-action h1 {
    font-weight: 500;
    max-width: 35rem;
    font-size: 3rem;
    line-height: 2.5rem;
}

.call-to-action h1 span {
    font-weight: 300;
    font-style: italic;
}

.call-to-action {
    width: 100%;
    height: 100%;
    display: flex;
    justify-content: flex-start;
    flex-direction: column;
    gap: 1rem;
}

.action-buttons {
    display: flex;
    gap: 1rem;
}

.btn-manage-tasks,
.btn-simple-task,
.btn-advanced-task,
.btn-add-task {
    padding: .5rem;
    background-color: var(--primary-color);
    color: var(--text-color);
    border: none;
    border-radius: 1rem;
    font-size: 1rem;
    font-weight: 500;
    cursor: pointer;
    border: .1rem solid var(--text-color);
    box-shadow: 5px 5px 1px var(--box-shadow-color);
    transition: box-shadow .3s ease;
}

.btn-manage-tasks:hover,
.btn-simple-task:hover,
.btn-advanced-task:hover,
.btn-add-task:hover {
    box-shadow: 8px 8px 1px var(--box-shadow-color);
}

.section-tasks {
    width: 100%;
    height: 50vh;
    padding: 4rem 10rem;
    display: flex;
    justify-content: space-evenly;
    align-items: center;
    background-color: var(--primary-color);
    border-top: solid .1rem var(--secondary-color);
}

.task-creation {
    width: 20rem;
    height: 16rem;
    display: flex;
    justify-content: center;
    flex-direction: column;
    align-items: center;
}

.task-inputs {
    display: flex;
    flex-direction: column;
    gap: .2rem;
}

.task-inputs input {
    width: 15rem;
    height: 2.5rem;
    padding: .8rem;
    border: none;
    border-radius: .8rem;
    background-color: var(--text-color);
    color: var(--secondary-color);
}

.task-inputs input:focus {
    outline: none;
}

.task-list {
    width: 20rem;
    height: 16rem;
    display: flex;
    justify-content: center;
    flex-direction: column;
    align-items: center;
    gap: .2rem;
}

.task-item {
    display: flex;
    justify-content: center;
    align-items: center;
    width: 15rem;
    height: 2.5rem;
    padding: .8rem;
    border: none;
    border-radius: .8rem;
    background-color: var(--text-color);
    color: var(--secondary-color);
}
